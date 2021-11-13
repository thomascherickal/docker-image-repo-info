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
-	[`nats-streaming:0.23.1`](#nats-streaming0231)
-	[`nats-streaming:0.23.1-alpine`](#nats-streaming0231-alpine)
-	[`nats-streaming:0.23.1-alpine3.14`](#nats-streaming0231-alpine314)
-	[`nats-streaming:0.23.1-linux`](#nats-streaming0231-linux)
-	[`nats-streaming:0.23.1-nanoserver`](#nats-streaming0231-nanoserver)
-	[`nats-streaming:0.23.1-nanoserver-1809`](#nats-streaming0231-nanoserver-1809)
-	[`nats-streaming:0.23.1-scratch`](#nats-streaming0231-scratch)
-	[`nats-streaming:0.23.1-windowsservercore`](#nats-streaming0231-windowsservercore)
-	[`nats-streaming:0.23.1-windowsservercore-1809`](#nats-streaming0231-windowsservercore-1809)
-	[`nats-streaming:0.23.1-windowsservercore-ltsc2016`](#nats-streaming0231-windowsservercore-ltsc2016)
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
$ docker pull nats-streaming@sha256:4b514c3c528a165308e4798df5f5e9d89b0e0814b312ff1ca397b19f77f50ee7
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine`

```console
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
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
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
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
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-scratch`

```console
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:5746ee094d87b59a38dacd578c153543176e620c2a27e4bd3cea9b8a568a1371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4ab09fe6525eef8718f86a6acc82a894c303ac4ad5e801ca6bcc13103aa01325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6133577c5d23012c70fba55177529173a992c27b7fd7faef03dcbcce4e814f57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1`

```console
$ docker pull nats-streaming@sha256:4b514c3c528a165308e4798df5f5e9d89b0e0814b312ff1ca397b19f77f50ee7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.1` - linux; amd64

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

### `nats-streaming:0.23.1` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1` - linux; arm variant v7

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

### `nats-streaming:0.23.1` - linux; arm64 variant v8

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

### `nats-streaming:0.23.1` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1-alpine`

```console
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine` - linux; arm64 variant v8

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

## `nats-streaming:0.23.1-alpine3.14`

```console
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.1-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-alpine3.14` - linux; arm64 variant v8

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

## `nats-streaming:0.23.1-linux`

```console
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.1-linux` - linux; amd64

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

### `nats-streaming:0.23.1-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-linux` - linux; arm variant v7

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

### `nats-streaming:0.23.1-linux` - linux; arm64 variant v8

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

## `nats-streaming:0.23.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.1-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.1-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1-scratch`

```console
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.1-scratch` - linux; amd64

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

### `nats-streaming:0.23.1-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-scratch` - linux; arm variant v7

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

### `nats-streaming:0.23.1-scratch` - linux; arm64 variant v8

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

## `nats-streaming:0.23.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:5746ee094d87b59a38dacd578c153543176e620c2a27e4bd3cea9b8a568a1371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.1-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.1-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4ab09fe6525eef8718f86a6acc82a894c303ac4ad5e801ca6bcc13103aa01325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.1-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.1-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6133577c5d23012c70fba55177529173a992c27b7fd7faef03dcbcce4e814f57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
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
$ docker pull nats-streaming@sha256:c33011e27cd41d096ca03defddda7c04f8dbd19117cbb6b239197837f05eac77
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6ba368573d98b4b0898b38f0f6a66978c9d2a1913747ab28ae683942c9e68493
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10392673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf7ca18fe0750634146c03f6e83080d0d8aae0fc695752133df686bf627f567`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:25:53 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:25:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:25:57 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:25:57 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:25:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6ad0849d761c25f08d32acdbc7ab9a7cea82140e761d1410d866e5f0467ca5`  
		Last Modified: Thu, 11 Nov 2021 02:26:47 GMT  
		Size: 7.6 MB (7577806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536585ec818899ef789e998f021327147a03d261d093e75449729694efe0659`  
		Last Modified: Thu, 11 Nov 2021 02:26:46 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:827769c2c72db48198ce3af76c9db804eb97bdaf4da35532e2e12de863ecf073
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9684872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f55c75446532df642d9d9d9737fb347f0be055f5711e96569f4b7a1dc0b67dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 02:19:35 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 02:19:41 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 02:19:42 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:19:43 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a233494649893864b622a009cbe802f9e0af2a7fc0a2b03d099985a6a444881`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 7.1 MB (7057003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5a5c40b1b132d4d1b71c272567d763d9826f54b8b8b2f9480f500ffb70e1a`  
		Last Modified: Thu, 11 Nov 2021 02:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:c4231db9ad0d02da2f931e8ba62590fb676adcfc44ddb3e34779919da1597833
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9476191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab78443c1bc85d17e593aed55723509f392f62a8ad0d24762ccc4ff648831b83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 Nov 2021 03:51:17 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 03:51:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1ae3356d830c22a1367ea4ba45f1d2868307c4c8deae13f9e89f0d1731a8fec7' ;; 		armhf) natsArch='arm6'; sha256='961f7f622ef790f909ce7e0521054a7ff1ffa7faaea0e0ca784855b0276fba93' ;; 		armv7) natsArch='arm7'; sha256='61992a8fae5617b14152bdb7d03e2379b8b7cd12b22c46fb7b37ffbe29cb75e7' ;; 		x86_64) natsArch='amd64'; sha256='34cc0d6ed58c8917aa432832afd25bb89ba9ea62ea595cec1846b014a659e4af' ;; 		x86) natsArch='386'; sha256='38fe4b22245a840279967520f9340a741ee0eea7a0fbe99a907a6a36041d323d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 11 Nov 2021 03:51:23 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 11 Nov 2021 03:51:24 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 03:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:51:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711b7a3449716edc54586eeffc6e034f832aefc87a4368017fc0d021ca305f46`  
		Last Modified: Thu, 11 Nov 2021 03:53:13 GMT  
		Size: 7.0 MB (7045350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9e0f8ca5c19450374a30999d004e73332cf129c2a95ab0d4027105daac18f`  
		Last Modified: Thu, 11 Nov 2021 03:53:09 GMT  
		Size: 422.0 B  
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
$ docker pull nats-streaming@sha256:4b514c3c528a165308e4798df5f5e9d89b0e0814b312ff1ca397b19f77f50ee7
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:be28d4c5d312498a5e7e11308efb9c66b85f6ac334ac4ea12f3bd843ac1870a3
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
$ docker pull nats-streaming@sha256:45e8441fe6b0aa39698fb860f7fd04084794a4f2a8e0a7cfff5370d747421177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6771824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:048a80f9c4772310915e26da2cc8319b434a2afad12fa851700f836bbeee2632`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 11 Nov 2021 02:20:01 GMT
COPY file:cafe128f6bc79fc96153c40f19543236e6e7322e16b97f5ef4afff43efd93e34 in /nats-streaming-server 
# Thu, 11 Nov 2021 02:20:02 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 11 Nov 2021 02:20:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:44905e0151acd3106c434b83755483d9ec3225b7f1c369ec6f4b0a5607a50c89`  
		Last Modified: Thu, 11 Nov 2021 02:21:57 GMT  
		Size: 6.8 MB (6771824 bytes)  
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
$ docker pull nats-streaming@sha256:5746ee094d87b59a38dacd578c153543176e620c2a27e4bd3cea9b8a568a1371
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:4ab09fe6525eef8718f86a6acc82a894c303ac4ad5e801ca6bcc13103aa01325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:0ea07cf4b2da4c7a1ced27f9f3506a153ee220ed17906ed5aa68a9fd3f49f5b7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714273600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3d540e9eb5802e40de7e47a6f523157853ec04cac933b58ea93ffbe61a4520f`
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
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:15:00 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:15:01 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:15:52 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:17:27 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:17:28 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:30 GMT
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
	-	`sha256:5de4b13cb73393643756e028e81ed4518ed99ddce44bd534cd504e2843e72e51`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a16d7b61f54b6df0ab681fca0806d55f6af5dda0015578fee2a96ac0e3afe9`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255da47e93b0ef5c313f9928d70bc57a76120a51a4c4a682cdbb683ac601dcd6`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e441cc1424810e93d13ca88e49893791517ba6e4aff1a8c2302b92acbc16fff0`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 368.5 KB (368488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33df97304091ce40de1df3ca9c702c99916053dfa645ba53636c695b8e99864b`  
		Last Modified: Thu, 11 Nov 2021 02:21:01 GMT  
		Size: 7.8 MB (7772718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f6fe75cfa2d02fa51ef432e349751d4e82f4e969792a705d04bd324573b38`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1dc261e9f7d720a7c36aaf02f60b5e23af5dfe80c319a616b9ec6e3932e9e`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d500922632854f925bd88e89c161e0d3153fc722ad0be1dbf0075ed315d2`  
		Last Modified: Thu, 11 Nov 2021 02:20:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6133577c5d23012c70fba55177529173a992c27b7fd7faef03dcbcce4e814f57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:853581e44ab82fac79225d1aee21fc2e796eb9cc228696b32c646d6110df0cd4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285775941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f58635f017372bf4978762895af8a8b95e97d5c29df3f4162d75c454be661f54`
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
# Thu, 11 Nov 2021 02:17:52 GMT
ENV NATS_STREAMING_SERVER=0.23.1
# Thu, 11 Nov 2021 02:17:53 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.1/nats-streaming-server-v0.23.1-windows-amd64.zip
# Thu, 11 Nov 2021 02:17:54 GMT
ENV NATS_STREAMING_SERVER_SHASUM=72dc7ce44509dfd80c843dbe4f6f8b1d30ceca9cfa41526b3bbf45c5055cb080
# Thu, 11 Nov 2021 02:18:41 GMT
RUN Set-PSDebug -Trace 2
# Thu, 11 Nov 2021 02:20:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 11 Nov 2021 02:20:25 GMT
EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:20:26 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:20:26 GMT
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
	-	`sha256:5481794a21ca3112b6a0fd85561fb2d3b70c632434d809fb7631dbe0d603d995`  
		Last Modified: Thu, 11 Nov 2021 02:21:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3dc37fbc927aca5e3a376e11e4a6817eb280bd11ff94a8252abed4c2f1357`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b68de91b7edc7154ac25082ce2f15c94a15747d4ad76cc1b1a884a6f190560`  
		Last Modified: Thu, 11 Nov 2021 02:21:27 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673e6529e6b46089d4813bf49ed675070c9a9f4a9cbac34747995881f7fb5ef`  
		Last Modified: Thu, 11 Nov 2021 02:21:26 GMT  
		Size: 358.5 KB (358500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4d4e3c95c69db114fb425f83d020b1ea58824bb54c112849e8244f3eedddc9`  
		Last Modified: Thu, 11 Nov 2021 02:21:38 GMT  
		Size: 12.3 MB (12315228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fd0dc5754fef88ab55b7d8ed7fb75889bb0ec6b175bdf0973093685c5e4c82`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83dd97c04746fb5236ff8a1d9e8192a3ca56482d7d893f435762f782ac5ffde`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09f0d27dc43fe660a0d67bb0b635bb4f7c4acb58ec2d7e8fecd1fffa5f6d4f0`  
		Last Modified: Thu, 11 Nov 2021 02:21:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
