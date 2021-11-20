<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.23`](#nats-streaming023)
-	[`nats-streaming:0.23-alpine`](#nats-streaming023-alpine)
-	[`nats-streaming:0.23-alpine3.14`](#nats-streaming023-alpine314)
-	[`nats-streaming:0.23-linux`](#nats-streaming023-linux)
-	[`nats-streaming:0.23-nanoserver`](#nats-streaming023-nanoserver)
-	[`nats-streaming:0.23-nanoserver-1809`](#nats-streaming023-nanoserver-1809)
-	[`nats-streaming:0.23-scratch`](#nats-streaming023-scratch)
-	[`nats-streaming:0.23-windowsservercore`](#nats-streaming023-windowsservercore)
-	[`nats-streaming:0.23-windowsservercore-1809`](#nats-streaming023-windowsservercore-1809)
-	[`nats-streaming:0.23-windowsservercore-ltsc2016`](#nats-streaming023-windowsservercore-ltsc2016)
-	[`nats-streaming:0.23.2`](#nats-streaming0232)
-	[`nats-streaming:0.23.2-alpine`](#nats-streaming0232-alpine)
-	[`nats-streaming:0.23.2-alpine3.14`](#nats-streaming0232-alpine314)
-	[`nats-streaming:0.23.2-linux`](#nats-streaming0232-linux)
-	[`nats-streaming:0.23.2-nanoserver`](#nats-streaming0232-nanoserver)
-	[`nats-streaming:0.23.2-nanoserver-1809`](#nats-streaming0232-nanoserver-1809)
-	[`nats-streaming:0.23.2-scratch`](#nats-streaming0232-scratch)
-	[`nats-streaming:0.23.2-windowsservercore`](#nats-streaming0232-windowsservercore)
-	[`nats-streaming:0.23.2-windowsservercore-1809`](#nats-streaming0232-windowsservercore-1809)
-	[`nats-streaming:0.23.2-windowsservercore-ltsc2016`](#nats-streaming0232-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.14`](#nats-streamingalpine314)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.23`

```console
$ docker pull nats-streaming@sha256:60c5d2edb53c5ec836b812f8cdb55e8eea74bbffe6a1eea65546a546dd590230
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine`

```console
$ docker pull nats-streaming@sha256:1150bd754436cafbf9e840570f69ad6ed02d68fa46ebf46ba06d7b4fd26cdb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ccbdee1001f1217f8427450b395e6978f27a60caea09ed3a21105b2926dd2239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10401143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ea744d3652f9f6deb6f9efb270a386770cc5cb8a9aed8a42b140639b89c8ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:20 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 05:46:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 05:46:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 05:46:23 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 05:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:46:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff955a4cc71f9aa0f7c6d03ac6e3294eb0b5079277c7eb563670a9bb95a8e43d`  
		Last Modified: Sat, 13 Nov 2021 05:47:21 GMT  
		Size: 7.6 MB (7577742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6a7277c9a41b94b8667f7699d18910036b0b4d3161dcfe43e01f10a893f5df`  
		Last Modified: Sat, 13 Nov 2021 05:47:19 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2ea65296f4d72a98eaa30964dcddac89ffcadade4369476f3d9979e7642e3ca7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9484865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82942a55205f6b5ac08a69a6daa9b5ea103b35658db44cbc1f5fb91c31585e7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:47:02 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 10:47:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 10:47:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 10:47:08 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 10:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 10:47:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf0ef3d0e064b957a52152df7939005b7e081df91f026db3d2d0de7cddff5c`  
		Last Modified: Sat, 13 Nov 2021 10:48:57 GMT  
		Size: 7.0 MB (7045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a5cdab71e5f58e9c84b6e905b525e8a834b61749f898191fcae8ddcf04125`  
		Last Modified: Sat, 13 Nov 2021 10:48:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:22f854e32680ae7743f49b00846edebe31e8ba7df68c3f198fe6075408d0c453
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792a113b8d92d69ff1479f5427147dc7589b47476eb305008238bfd836e59b30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:15:21 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 00:15:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 00:15:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 00:15:27 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 00:15:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 00:15:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05923b68c5a6573ba372063616bf3a1a3a2a1a2e8ccaa36d02778b61c68aba`  
		Last Modified: Sat, 13 Nov 2021 00:16:16 GMT  
		Size: 6.9 MB (6945710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059df5a49c9020cbd9ff7660a051b720ea8d9fd7feafdbb2a67d7759e7345f52`  
		Last Modified: Sat, 13 Nov 2021 00:16:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine3.14`

```console
$ docker pull nats-streaming@sha256:1150bd754436cafbf9e840570f69ad6ed02d68fa46ebf46ba06d7b4fd26cdb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ccbdee1001f1217f8427450b395e6978f27a60caea09ed3a21105b2926dd2239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10401143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ea744d3652f9f6deb6f9efb270a386770cc5cb8a9aed8a42b140639b89c8ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:20 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 05:46:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 05:46:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 05:46:23 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 05:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:46:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff955a4cc71f9aa0f7c6d03ac6e3294eb0b5079277c7eb563670a9bb95a8e43d`  
		Last Modified: Sat, 13 Nov 2021 05:47:21 GMT  
		Size: 7.6 MB (7577742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6a7277c9a41b94b8667f7699d18910036b0b4d3161dcfe43e01f10a893f5df`  
		Last Modified: Sat, 13 Nov 2021 05:47:19 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2ea65296f4d72a98eaa30964dcddac89ffcadade4369476f3d9979e7642e3ca7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9484865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82942a55205f6b5ac08a69a6daa9b5ea103b35658db44cbc1f5fb91c31585e7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:47:02 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 10:47:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 10:47:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 10:47:08 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 10:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 10:47:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf0ef3d0e064b957a52152df7939005b7e081df91f026db3d2d0de7cddff5c`  
		Last Modified: Sat, 13 Nov 2021 10:48:57 GMT  
		Size: 7.0 MB (7045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a5cdab71e5f58e9c84b6e905b525e8a834b61749f898191fcae8ddcf04125`  
		Last Modified: Sat, 13 Nov 2021 10:48:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:22f854e32680ae7743f49b00846edebe31e8ba7df68c3f198fe6075408d0c453
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792a113b8d92d69ff1479f5427147dc7589b47476eb305008238bfd836e59b30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:15:21 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 00:15:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 00:15:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 00:15:27 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 00:15:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 00:15:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05923b68c5a6573ba372063616bf3a1a3a2a1a2e8ccaa36d02778b61c68aba`  
		Last Modified: Sat, 13 Nov 2021 00:16:16 GMT  
		Size: 6.9 MB (6945710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059df5a49c9020cbd9ff7660a051b720ea8d9fd7feafdbb2a67d7759e7345f52`  
		Last Modified: Sat, 13 Nov 2021 00:16:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-linux`

```console
$ docker pull nats-streaming@sha256:aedf11f864561ec5cfed5723a27af2cddc4156e39e5508ea9ca8951eeb94c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-scratch`

```console
$ docker pull nats-streaming@sha256:aedf11f864561ec5cfed5723a27af2cddc4156e39e5508ea9ca8951eeb94c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore`

```console
$ docker pull nats-streaming@sha256:24b7c3eef25b0f52a4eeceefcaada76227c649e3e2ae98e4b3a570d59a8a6dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:eb16841747bfd3b80f7fc2d0480040c15674192838c012b4d80cc02027f8f0ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9623c2fc66e12e8a3e0230fd2f17d0127a8b7f2036b872c1d669dbfa0d6d693d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2`

```console
$ docker pull nats-streaming@sha256:d87eb7dbf435444448fdf288d24882a3a31d8dea0529f0c94e911d530c23f09a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.2` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-alpine`

```console
$ docker pull nats-streaming@sha256:34d0fcb07d0e15385d523ca0e30d8bdf0029b7efe77316a57f8dd643b67c73f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.23.2-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-alpine3.14`

```console
$ docker pull nats-streaming@sha256:34d0fcb07d0e15385d523ca0e30d8bdf0029b7efe77316a57f8dd643b67c73f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.23.2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-linux`

```console
$ docker pull nats-streaming@sha256:d7168a2bd51baf6f5dd7a67da3f8d60a8fc2b9b15ba291751b8ce182d2a52888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.23.2-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-nanoserver`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.2-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.2-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-scratch`

```console
$ docker pull nats-streaming@sha256:d7168a2bd51baf6f5dd7a67da3f8d60a8fc2b9b15ba291751b8ce182d2a52888
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.23.2-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore`

```console
$ docker pull nats-streaming@sha256:24b7c3eef25b0f52a4eeceefcaada76227c649e3e2ae98e4b3a570d59a8a6dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.2-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:eb16841747bfd3b80f7fc2d0480040c15674192838c012b4d80cc02027f8f0ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.2-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.2-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9623c2fc66e12e8a3e0230fd2f17d0127a8b7f2036b872c1d669dbfa0d6d693d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:1150bd754436cafbf9e840570f69ad6ed02d68fa46ebf46ba06d7b4fd26cdb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ccbdee1001f1217f8427450b395e6978f27a60caea09ed3a21105b2926dd2239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10401143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ea744d3652f9f6deb6f9efb270a386770cc5cb8a9aed8a42b140639b89c8ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:20 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 05:46:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 05:46:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 05:46:23 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 05:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:46:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff955a4cc71f9aa0f7c6d03ac6e3294eb0b5079277c7eb563670a9bb95a8e43d`  
		Last Modified: Sat, 13 Nov 2021 05:47:21 GMT  
		Size: 7.6 MB (7577742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6a7277c9a41b94b8667f7699d18910036b0b4d3161dcfe43e01f10a893f5df`  
		Last Modified: Sat, 13 Nov 2021 05:47:19 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2ea65296f4d72a98eaa30964dcddac89ffcadade4369476f3d9979e7642e3ca7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9484865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82942a55205f6b5ac08a69a6daa9b5ea103b35658db44cbc1f5fb91c31585e7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:47:02 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 10:47:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 10:47:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 10:47:08 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 10:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 10:47:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf0ef3d0e064b957a52152df7939005b7e081df91f026db3d2d0de7cddff5c`  
		Last Modified: Sat, 13 Nov 2021 10:48:57 GMT  
		Size: 7.0 MB (7045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a5cdab71e5f58e9c84b6e905b525e8a834b61749f898191fcae8ddcf04125`  
		Last Modified: Sat, 13 Nov 2021 10:48:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:22f854e32680ae7743f49b00846edebe31e8ba7df68c3f198fe6075408d0c453
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792a113b8d92d69ff1479f5427147dc7589b47476eb305008238bfd836e59b30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:15:21 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 00:15:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 00:15:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 00:15:27 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 00:15:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 00:15:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05923b68c5a6573ba372063616bf3a1a3a2a1a2e8ccaa36d02778b61c68aba`  
		Last Modified: Sat, 13 Nov 2021 00:16:16 GMT  
		Size: 6.9 MB (6945710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059df5a49c9020cbd9ff7660a051b720ea8d9fd7feafdbb2a67d7759e7345f52`  
		Last Modified: Sat, 13 Nov 2021 00:16:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:1150bd754436cafbf9e840570f69ad6ed02d68fa46ebf46ba06d7b4fd26cdb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ccbdee1001f1217f8427450b395e6978f27a60caea09ed3a21105b2926dd2239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10401143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ea744d3652f9f6deb6f9efb270a386770cc5cb8a9aed8a42b140639b89c8ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:46:20 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 05:46:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 05:46:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 05:46:23 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 05:46:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:46:24 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff955a4cc71f9aa0f7c6d03ac6e3294eb0b5079277c7eb563670a9bb95a8e43d`  
		Last Modified: Sat, 13 Nov 2021 05:47:21 GMT  
		Size: 7.6 MB (7577742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6a7277c9a41b94b8667f7699d18910036b0b4d3161dcfe43e01f10a893f5df`  
		Last Modified: Sat, 13 Nov 2021 05:47:19 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:983f8ac2dbbaa85241dbc5508ee63b554e7ac9952787ddb8c11565fe8fa6f89d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9694130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428fa782d5b97614b699deec16e4b3715fe3df66e91d7c27b27104a5534c9f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 19 Nov 2021 23:49:35 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Fri, 19 Nov 2021 23:49:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 19 Nov 2021 23:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 19 Nov 2021 23:49:41 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Nov 2021 23:49:42 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824cebd74c6dc7b249f375f4f8b9b003e37db5170f8a26342ed408ae5f39da31`  
		Last Modified: Fri, 19 Nov 2021 23:51:24 GMT  
		Size: 7.1 MB (7058316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898a9271af9b0a02e91bab485a625e6bba3437f8ed1953bd6497c5a6fee966`  
		Last Modified: Fri, 19 Nov 2021 23:51:19 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2ea65296f4d72a98eaa30964dcddac89ffcadade4369476f3d9979e7642e3ca7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9484865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82942a55205f6b5ac08a69a6daa9b5ea103b35658db44cbc1f5fb91c31585e7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 10:47:02 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 10:47:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 10:47:08 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 10:47:08 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 10:47:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 10:47:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdf0ef3d0e064b957a52152df7939005b7e081df91f026db3d2d0de7cddff5c`  
		Last Modified: Sat, 13 Nov 2021 10:48:57 GMT  
		Size: 7.0 MB (7045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a5cdab71e5f58e9c84b6e905b525e8a834b61749f898191fcae8ddcf04125`  
		Last Modified: Sat, 13 Nov 2021 10:48:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:22f854e32680ae7743f49b00846edebe31e8ba7df68c3f198fe6075408d0c453
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9663831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792a113b8d92d69ff1479f5427147dc7589b47476eb305008238bfd836e59b30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:15:21 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Sat, 13 Nov 2021 00:15:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 13 Nov 2021 00:15:27 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 13 Nov 2021 00:15:27 GMT
EXPOSE 4222 8222
# Sat, 13 Nov 2021 00:15:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 00:15:29 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05923b68c5a6573ba372063616bf3a1a3a2a1a2e8ccaa36d02778b61c68aba`  
		Last Modified: Sat, 13 Nov 2021 00:16:16 GMT  
		Size: 6.9 MB (6945710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059df5a49c9020cbd9ff7660a051b720ea8d9fd7feafdbb2a67d7759e7345f52`  
		Last Modified: Sat, 13 Nov 2021 00:16:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:60c5d2edb53c5ec836b812f8cdb55e8eea74bbffe6a1eea65546a546dd590230
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:aedf11f864561ec5cfed5723a27af2cddc4156e39e5508ea9ca8951eeb94c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:aedf11f864561ec5cfed5723a27af2cddc4156e39e5508ea9ca8951eeb94c745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:e87c5530f8f41a086cdc5a60a7952e4bb11d3ca3a8beaab403cbe7a0eb032bc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7292639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12ab80593593a3b7baf81e41464f957af84d4b10476100bcdb56dd34283eccac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:26:24 GMT
COPY file:58b77819476f9bf3c103371566b6765337aa77273f2b32e034ed7683e20d46e9 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:26:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:26:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:26:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:1bb27f8812fc2df86c3a265f022727bcde08f73d26718d1305bdb495155e5874`  
		Last Modified: Thu, 11 Nov 2021 02:27:06 GMT  
		Size: 7.3 MB (7292639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:0c1a07390ec1c002d89b5bcd0d0048c95f33f859d53b607ffdc16678e3f79bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6774516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1392e1316cac3fc870ec9cd90c7973466ed1433895aee0166a624b060262b6b5`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 19 Nov 2021 23:50:00 GMT
COPY file:d86d6a12a47b28bc562444b508d1508f4f436aa57b4f9785d2f72f13991058d9 in /nats-streaming-server 
# Fri, 19 Nov 2021 23:50:00 GMT
EXPOSE 4222 8222
# Fri, 19 Nov 2021 23:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 19 Nov 2021 23:50:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ada5d2acf52444276ec7168ad03307d61f3ac5bb2e33825f280ba40e265f0533`  
		Last Modified: Fri, 19 Nov 2021 23:51:55 GMT  
		Size: 6.8 MB (6774516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:54afe06d8d830b4343f8619b4467eb8baa2a827273ef68641ab0d50a9577a03c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6762593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab9e15811b57f6732ce60f10656b3639e807cedf80e4cc6d8652a8ec7da94382`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:51:47 GMT
COPY file:b00a3b3f091d4aa33ae4542e7ae295593bc122e9dff95ac33ea4d2b1efa934be in /nats-streaming-server 
# Thu, 11 Nov 2021 03:51:47 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:48 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:51:48 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:abbad007ce8318ff583bdfe434b016de78146bb8e793beeda9da1ca38e6982da`  
		Last Modified: Thu, 11 Nov 2021 03:53:44 GMT  
		Size: 6.8 MB (6762593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:3ab1dc9a52da2a1fd03534fa4a603a387975bec504ab4ce52215dcf1e0569752
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6663494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58ef5a6636609fa968037360eeb7ff983841459f566429d6c58540b42a5e29a3`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 03:00:43 GMT
COPY file:96e57a079c6048b5be141b65e2f2e6fbe0b082f2fdbb12152319587bca197d2e in /nats-streaming-server 
# Thu, 11 Nov 2021 03:00:44 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:00:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 03:00:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:d97fbb66ba3557ddd9c6f8794eec24682187d368eb6c337de60a84c6e1a66c91`  
		Last Modified: Thu, 11 Nov 2021 03:01:45 GMT  
		Size: 6.7 MB (6663494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:24b7c3eef25b0f52a4eeceefcaada76227c649e3e2ae98e4b3a570d59a8a6dc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:eb16841747bfd3b80f7fc2d0480040c15674192838c012b4d80cc02027f8f0ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:6f64bd15b581a70d6dfe857f3b44772d1757080d32fd1b99a19d8807def213d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714275444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c386ba25006af61aa18afb0f4ba34e37130c67698f7f702f6b8e73d1d80c71`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:00:40 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:15:12 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:15:13 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:15:14 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:16:03 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:17:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:17:40 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:17:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3df59793c391e0eb7e6a2ddb65801dfa94397b370daa52d04e242ba0274e3d`  
		Last Modified: Wed, 10 Nov 2021 17:06:13 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8527719d6ca5920291f35175b6c32f82952164d42b880f25f57e2ab782716f6`  
		Last Modified: Sat, 20 Nov 2021 00:21:14 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5527fe17246c670fd28071726d0070083f7817bf7a283ee290a4a3578be1c529`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa3900f098cee74ded07ca4efb271ae252d7eccb30ab9f2b5a6ebef3b90ffb`  
		Last Modified: Sat, 20 Nov 2021 00:21:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabfbc5f736cd2fb608eab7684b37557bba10062b0907a5f1cfb3a82eaf527a`  
		Last Modified: Sat, 20 Nov 2021 00:21:12 GMT  
		Size: 368.5 KB (368487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b742456a9e3d889a1da0049b32c41d9d8c0bcfe02c18bc2e5cb8799f0f453c`  
		Last Modified: Sat, 20 Nov 2021 00:21:20 GMT  
		Size: 7.8 MB (7774527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c68e60ff51543de0cd01cacdc9b50197cf509ff41cde3836443fbce7bf83467`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919e7cdd885b3a08ac5cea5bd5ac952f6ba0788a0f0237c536fd480fd5bae9b7`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab6f9a5538b2a14c942766e01516128ae2c95e811132f8101ac366b93f7b6a`  
		Last Modified: Sat, 20 Nov 2021 00:21:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:9623c2fc66e12e8a3e0230fd2f17d0127a8b7f2036b872c1d669dbfa0d6d693d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:a8754ad059b322a076af9cec4038bd0105348d25833189928402564118e1d5ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6281259279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b89781f458ba786a9ef0842c06ad7b3548e55e6f5d4a0595b002962db220d3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 17:03:18 GMT
ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:18:06 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 00:18:07 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.2/nats-streaming-server-v0.23.2-windows-amd64.zip
# Sat, 20 Nov 2021 00:18:08 GMT
ENV NATS_STREAMING_SERVER_SHASUM=b28dc8e1565d6fece68781515f759b0ed870831cdf2f7925cff7cf9acb44e7ec
# Sat, 20 Nov 2021 00:18:55 GMT
RUN Set-PSDebug -Trace 2
# Sat, 20 Nov 2021 00:20:32 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Sat, 20 Nov 2021 00:20:33 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:20:34 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:20:35 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5db4062c12269959ca71caf00b70e9baebf61b90c49c74db0e2cdb04cf83e8`  
		Last Modified: Wed, 10 Nov 2021 17:06:51 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5340cf4b5229cb811aded6948a78dd070b1dcd7d9c79a163dd4bcdfdf6e1f`  
		Last Modified: Sat, 20 Nov 2021 00:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0992c1fb2bdb48b803b13b4a53e6c0cb2fdd68a80612186a9c860a467f826463`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1f397ce101e6984fb89ec5963b486f147cc90083474ee83e5ebabb5ed34439`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8ce7e3e4df470099c34c35a291bbc11ebee219db5322ff65ab4d19856a864d`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 359.0 KB (359036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed4996f5a535c518a031301e7d66d2f866efa97ec83dde420c909ae39c7bc4a`  
		Last Modified: Sat, 20 Nov 2021 00:21:47 GMT  
		Size: 7.8 MB (7798409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfc383e29d1dc876d8581691fc650f37a769e12321b24db3221b4e9243f7a11`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1db010ba3db16a3ebeb3a7ff12851946f6e49c72e22f1082743768ef2e0f9`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a31dde888d46608b0de9acdfd5988c297ccd2b1187c681185687b27b283dfd`  
		Last Modified: Sat, 20 Nov 2021 00:21:45 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
