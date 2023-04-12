<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.25`](#nats-streaming025)
-	[`nats-streaming:0.25-alpine`](#nats-streaming025-alpine)
-	[`nats-streaming:0.25-alpine3.17`](#nats-streaming025-alpine317)
-	[`nats-streaming:0.25-linux`](#nats-streaming025-linux)
-	[`nats-streaming:0.25-nanoserver`](#nats-streaming025-nanoserver)
-	[`nats-streaming:0.25-nanoserver-1809`](#nats-streaming025-nanoserver-1809)
-	[`nats-streaming:0.25-scratch`](#nats-streaming025-scratch)
-	[`nats-streaming:0.25-windowsservercore`](#nats-streaming025-windowsservercore)
-	[`nats-streaming:0.25-windowsservercore-1809`](#nats-streaming025-windowsservercore-1809)
-	[`nats-streaming:0.25.3`](#nats-streaming0253)
-	[`nats-streaming:0.25.3-alpine`](#nats-streaming0253-alpine)
-	[`nats-streaming:0.25.3-alpine3.17`](#nats-streaming0253-alpine317)
-	[`nats-streaming:0.25.3-linux`](#nats-streaming0253-linux)
-	[`nats-streaming:0.25.3-nanoserver`](#nats-streaming0253-nanoserver)
-	[`nats-streaming:0.25.3-nanoserver-1809`](#nats-streaming0253-nanoserver-1809)
-	[`nats-streaming:0.25.3-scratch`](#nats-streaming0253-scratch)
-	[`nats-streaming:0.25.3-windowsservercore`](#nats-streaming0253-windowsservercore)
-	[`nats-streaming:0.25.3-windowsservercore-1809`](#nats-streaming0253-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.17`](#nats-streamingalpine317)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.25`

```console
$ docker pull nats-streaming@sha256:0d6971f0a7191bd2fe3d762045e097da478e59c1305223c9fb9323e35c240f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine3.17`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine3.17` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-linux`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-scratch`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3`

```console
$ docker pull nats-streaming@sha256:0d6971f0a7191bd2fe3d762045e097da478e59c1305223c9fb9323e35c240f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25.3` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-alpine`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.3-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-alpine3.17`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.3-alpine3.17` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-linux`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.3-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-nanoserver`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25.3-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25.3-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-scratch`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.3-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-windowsservercore`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25.3-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.3-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:0.25.3-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.17`

```console
$ docker pull nats-streaming@sha256:11e67880a7530e79b3d7732acd4a2fec7a87a99dfe99ff1ae34a02f9b0036e63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.17` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33ab0f0d21265a786135545d46035f7a4c315ea0ca84d652295bec764c2d88a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11326555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ccfcbad20611d1aa935b9ad0352190a45aa38d8a89a3c87895ea8b42502ec0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:34:42 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 22:34:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 22:34:45 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 22:34:45 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 22:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:34:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5d37fb7cb119872af61de93adacff08235e50a90ffea52f6daa9f9e318a45b`  
		Last Modified: Wed, 29 Mar 2023 22:35:02 GMT  
		Size: 8.0 MB (7951572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d051177506124f7e3e7e3ee69487686f7ef4b0e98ce0756b40cdff883f8ad221`  
		Last Modified: Wed, 29 Mar 2023 22:35:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:2b872c9f38fbaa8ccd86aae99ff49be7ca0081947ff402419b4908daf58019e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10725973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85cf282fbb53d74f70eb62b53a208af332a235cc98c5c913b9c2ce328695079c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:27:45 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:27:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:27:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:27:48 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:27:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99adc85b7a7f0c407e58670682e492d2ed4d84e3ab1bb7027956969d00ebfc71`  
		Last Modified: Wed, 29 Mar 2023 19:28:01 GMT  
		Size: 7.6 MB (7614751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4909158433ab6374c50735598fc1b8ced59a9783484d5d81b17f79e340f51`  
		Last Modified: Wed, 29 Mar 2023 19:28:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:3dd42a0204775da869e619716598df034fdc2dc745fe54733e05283be46959a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10475540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc61fa844612cd4e06d2f86ec59df937bb440d8bf4d9136d8e6f31c9e6af6b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:29 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 29 Mar 2023 19:25:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Wed, 29 Mar 2023 19:25:32 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:32 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ff327778aa8c8454a9938f941121fa97bd7b586285cb6a129c21cd04d644d6`  
		Last Modified: Wed, 29 Mar 2023 19:26:04 GMT  
		Size: 7.6 MB (7606603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40c1e330b4e950e4a13732095c4ed8bc3229d2036ab640e7211a90fc501e80a`  
		Last Modified: Wed, 29 Mar 2023 19:26:03 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ebc1dff84a15a9554c46b2cc905d4f1d212ddd6046cd7be5f7016e6f83e4d16c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10569180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a816d03c173976a973252506f4833cabd4a30fac73057d954bc92e059132339`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:18:46 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Thu, 30 Mar 2023 04:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='250dbab0595befb22a54804ec9be48537f22da0b6a5970e984d84c28d19f70d5' ;; 		armhf) natsArch='arm6'; sha256='27c74e261ccd1374da227e8c31184a8e98d0820bdd916e9a681be7fba12f7f09' ;; 		armv7) natsArch='arm7'; sha256='3db62df2019c947b54ea943ecaa5d1e34db6855247e53ec7c8ad46d0c206a6c4' ;; 		x86_64) natsArch='amd64'; sha256='ac5beb0e820af18e422bef12200012d86237b98872e0ed48c985426315b02cbb' ;; 		x86) natsArch='386'; sha256='887527bb48ab6029cbc1583cfd09e608148342e50e71851dbfa4c88aefb3fd39' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 30 Mar 2023 04:18:48 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 30 Mar 2023 04:18:48 GMT
EXPOSE 4222 8222
# Thu, 30 Mar 2023 04:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:18:49 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f3992e784b927acf49dc5a0cc6b1664716638d8f7dbe1e0700668abf27e02f`  
		Last Modified: Thu, 30 Mar 2023 04:19:03 GMT  
		Size: 7.3 MB (7306905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077ed6bc29c4733d67edff9c646c2f8ea49b889a895ea879b3d9cfd24aceebb`  
		Last Modified: Thu, 30 Mar 2023 04:19:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:0d6971f0a7191bd2fe3d762045e097da478e59c1305223c9fb9323e35c240f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9666436fc76ec939ffd8388a57f2593c71da1654a685edcf7f42e4f738221ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:3db51687d7a4e9688efbfa7c42f197e7fe93dbd87980f4757f82ad89548e0576
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114587969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3c8ce00dc9d3fb76eca0b0282234377d2d16b0851f8f821d7e2bda3fd7b68f`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:54:16 GMT
RUN cmd /S /C #(nop) COPY file:849c881d7b0e5994559eaa48b9cc851618ba91f60a4b0e8cb48b89862fd563c8 in C:\nats-streaming-server.exe 
# Wed, 12 Apr 2023 02:54:18 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:20 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d340e7e81d7fb1725f887a5504a11e7a0918fed033edcb16ff9a2ec0d84ed33`  
		Last Modified: Wed, 12 Apr 2023 02:55:04 GMT  
		Size: 7.8 MB (7794469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b4c5f1872b62bf23b5fa895aa9a0278c048ea179c2e19d4e73315178754fcc`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9036e5beba504789a120795d7130d2a145bfaa5b26cb31e90f74869ff2acddba`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961e9b64fbab719cdfb82b8bc7824591ff8ce559aaf6c1f50141e36278d3a6c5`  
		Last Modified: Wed, 12 Apr 2023 02:55:02 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:73f07f50ce952ce448048e75d494ee6ed95eae0ad7275b712e8214552113960a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:1a8745712d00a54265c8552863b8d15a568b138368f4fcb090c075e361124c14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a48bccf54f8248bddd0509da6d1cc1fe8b97638f6120c98e4c9fb191f6f1723`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:31:40 GMT
COPY file:379a895964ce5e0c1d6e137ee5ee8f0cbfb7fdbb8cb20ace28a5de2e106737eb in /nats-streaming-server 
# Thu, 12 Jan 2023 19:31:40 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:31:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:31:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:27e278d5ae53768a5d47168e25eb6824c8445f2866af5ea11943739d93ce14dd`  
		Last Modified: Thu, 12 Jan 2023 19:32:24 GMT  
		Size: 7.7 MB (7666171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:01c1adc9b48bd0eaf83deed2c829ba46ca7e195e485c64b91dfe60155372b90d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7329068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2496f5e117da007615485710e84d73fc0a353a004d88ce6bd42efbb52c5d4b92`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 14 Mar 2023 01:40:38 GMT
COPY file:1214576567fc0305b3b6ac3e280bb8d103f74aee2edde4b083a56167e41f0ed6 in /nats-streaming-server 
# Tue, 14 Mar 2023 01:40:38 GMT
EXPOSE 4222 8222
# Tue, 14 Mar 2023 01:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 14 Mar 2023 01:40:38 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c76ebdda577d691c315b52196919494198f01e7e8a34dac185a83423d3954e4f`  
		Last Modified: Thu, 12 Jan 2023 18:58:31 GMT  
		Size: 7.3 MB (7329068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:bcefecfcb6986469865e3d3d3fbb31f8101c56a77b76a3c3cb076ae08ab06ae8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7318728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6202a592a6aad13e30bce4ac90570fe13d8f28740d9ca9b75958c204953b43bd`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Mar 2023 19:25:37 GMT
COPY file:58653f0fa67e6667e5ec024a8b7912bc01a12570dac2c7550d04c2e617252bf1 in /nats-streaming-server 
# Wed, 29 Mar 2023 19:25:37 GMT
EXPOSE 4222 8222
# Wed, 29 Mar 2023 19:25:37 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Mar 2023 19:25:37 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:edc8f5310312ee44896e1639c9af8d17c77c9fc7cfad03f8c1268ab57def8348`  
		Last Modified: Thu, 12 Jan 2023 19:12:45 GMT  
		Size: 7.3 MB (7318728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:56dfb1bed3b56ea0b72be1b79a49422abdde1189777ebfb55eda7223819eb6d3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7019428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7533789a178d97f2445ccdb62e46c98a1cec7249342ad21b5c40f38ee0652bff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 12 Jan 2023 19:49:56 GMT
COPY file:33b7386a5076cd63bc03cf5c4de0f89afe8fd8034e8fd3a792715c6cb567514b in /nats-streaming-server 
# Thu, 12 Jan 2023 19:49:56 GMT
EXPOSE 4222 8222
# Thu, 12 Jan 2023 19:49:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 12 Jan 2023 19:49:56 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b7cbef42b1eb11c382f636b05c7fea54926364454d6b2727ea8e52f63785a536`  
		Last Modified: Thu, 12 Jan 2023 19:50:42 GMT  
		Size: 7.0 MB (7019428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:08798cf762b1971f7733e42d08e6b035fca00c85df8d6eed35566a9b42fb43e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats-streaming@sha256:f4e06e330b3f5b04a0b4869e1475a1be8dabf7d0c555d31638cf63c2f7ce8e05
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2079954789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:730388aafd3fb6e94a5fbb3ca2923d908a88a70987542cd8f3aec0875aa6e422`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:48:58 GMT
ENV NATS_STREAMING_SERVER=0.25.3
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.3/nats-streaming-server-v0.25.3-windows-amd64.zip
# Wed, 12 Apr 2023 02:49:00 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b25aab68b84cba76e3edec5d524d2a792f460127d159ecb4d2e6168c7635c10c
# Wed, 12 Apr 2023 02:51:00 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:54:00 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:54:01 GMT
EXPOSE 4222 8222
# Wed, 12 Apr 2023 02:54:02 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 Apr 2023 02:54:04 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d307d893fbeb91714142851c9b77274bd7d8558c0130d095791519f1b00993`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf34831b97e978505e0c96019e7893d245a7ccd9aab9895bb0a58b9ccf33dfca`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dfeeb40c1ca2e0d61377dd9a76d1be12884552db49acaa27b01b952472ba92`  
		Last Modified: Wed, 12 Apr 2023 02:54:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169dda2907fa6bd3400d8e5d242650dcad43a8e7f28d768eaac7d4cf05f35fc2`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 495.5 KB (495517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1b747c5b3dcc333c8277218e668fe8a63909452f67ab1bd68bb5ad00b66a94`  
		Last Modified: Wed, 12 Apr 2023 02:54:49 GMT  
		Size: 8.2 MB (8156762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8066f145c6b9d10d87a1e85b0e94fd3b8e70892bd838575c746abf7bce634c`  
		Last Modified: Wed, 12 Apr 2023 02:54:47 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ff92a44dfc6bd0976cc42f1b4f0eb81db01f740d36ad047e6ca87b4e861842`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68ea5be3292c7ee712b067942f62560398f0d91609a49f72c4bddba19d5879d`  
		Last Modified: Wed, 12 Apr 2023 02:54:46 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
