<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.24`](#nats-streaming024)
-	[`nats-streaming:0.24-alpine`](#nats-streaming024-alpine)
-	[`nats-streaming:0.24-alpine3.15`](#nats-streaming024-alpine315)
-	[`nats-streaming:0.24-linux`](#nats-streaming024-linux)
-	[`nats-streaming:0.24-nanoserver`](#nats-streaming024-nanoserver)
-	[`nats-streaming:0.24-nanoserver-1809`](#nats-streaming024-nanoserver-1809)
-	[`nats-streaming:0.24-scratch`](#nats-streaming024-scratch)
-	[`nats-streaming:0.24-windowsservercore`](#nats-streaming024-windowsservercore)
-	[`nats-streaming:0.24-windowsservercore-1809`](#nats-streaming024-windowsservercore-1809)
-	[`nats-streaming:0.24.1`](#nats-streaming0241)
-	[`nats-streaming:0.24.1-alpine`](#nats-streaming0241-alpine)
-	[`nats-streaming:0.24.1-alpine3.15`](#nats-streaming0241-alpine315)
-	[`nats-streaming:0.24.1-linux`](#nats-streaming0241-linux)
-	[`nats-streaming:0.24.1-nanoserver`](#nats-streaming0241-nanoserver)
-	[`nats-streaming:0.24.1-nanoserver-1809`](#nats-streaming0241-nanoserver-1809)
-	[`nats-streaming:0.24.1-scratch`](#nats-streaming0241-scratch)
-	[`nats-streaming:0.24.1-windowsservercore`](#nats-streaming0241-windowsservercore)
-	[`nats-streaming:0.24.1-windowsservercore-1809`](#nats-streaming0241-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.15`](#nats-streamingalpine315)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.24`

```console
$ docker pull nats-streaming@sha256:46214f4467deabc181784961b7819d2d094c1b3c1b9ac2507548d054a5c80200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-scratch`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1`

```console
$ docker pull nats-streaming@sha256:46214f4467deabc181784961b7819d2d094c1b3c1b9ac2507548d054a5c80200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.1` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-alpine`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.1-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-alpine3.15`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.1-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-linux`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.1-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-nanoserver`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.1-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.1-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-scratch`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.1-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-windowsservercore`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.1-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.1-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:d3efe1bfff119cc0b2aa01b8c63144ba2ef137d49b797f347235ab4d13466924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:6132b676fbfb795fdfad0237d54fe96f712255a8a4a4a9e222c5a948cba59af4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10135327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d26790d12f236b4762f0afa25bb9a333eff705c926b86cfb9e8a041b175cc3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 19:19:49 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 19:19:53 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 19:19:53 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 19:19:53 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e7c7813b8aca3e9bcf9e2f771726eeedd068019169a750b3c8f4b2ed058ad`  
		Last Modified: Mon, 07 Feb 2022 19:21:01 GMT  
		Size: 7.3 MB (7316491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc4bff4e7ff0fefffe814efd40ffd59cc778f69c53d9e7e8f2d9e196743269a`  
		Last Modified: Mon, 07 Feb 2022 19:21:00 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18cf2d6cb954531a04883474e1a4495d16617d9fce0e0e8ccf9dbc09bc81f044
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a23b9861acbc12ea9dc3f850b23e8bc58e9966a0fac9a685446c7ba1246e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:49:35 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:49:40 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:49:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:49:41 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c11df6665d6d85ed49a6ab5685064b41edcca9717c00afc26c3106e122115ad`  
		Last Modified: Mon, 07 Feb 2022 18:51:26 GMT  
		Size: 6.8 MB (6833017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e7e78bab115f57f3a58b30be1639482f73dcc1701edae9df6d2b5aaf6b908`  
		Last Modified: Mon, 07 Feb 2022 18:51:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:4f708efbbc8ef6b0443423966ef9553145aac55ee41de93fd8dfb66f2379417a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9258267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3d7ea92c003ec567ac890b9b28bb19b4022fffa53f55e45ae8ca1b8cce48077`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:57:42 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:57:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:57:47 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:57:48 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:57:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:57:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7d7d65a051d7949dceca75221ae3ee6e55ee899852268b21017a89a3f1550`  
		Last Modified: Mon, 07 Feb 2022 18:59:37 GMT  
		Size: 6.8 MB (6823079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5657e27eafd3cae8ae8a24b7421dacc32123465721e8a842bbb8f3c4d71696a1`  
		Last Modified: Mon, 07 Feb 2022 18:59:32 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28a4807fc7a2b86df590affe751196026977d7480139fb8ca53511fe90e55bc9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9462283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70e8ff3f454f046dc7ee1f2dce1a146bfb3e61dfd433c841447ea82f8c18278`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Feb 2022 18:40:04 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 18:40:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4f523a0562e61b46965ab7ebf0a0a84eced6152c43a85b04d4820afa4630fd4a' ;; 		armhf) natsArch='arm6'; sha256='cfc10c9c58325b862f38b4c1c08ee492d05cdf4e848aa24068dd8aeb083abda5' ;; 		armv7) natsArch='arm7'; sha256='e72a91c6904bf42641e1737c3529c220ff93b34f055c7379a0bbdc7ba1529b9b' ;; 		x86_64) natsArch='amd64'; sha256='8c5ec55312c1cb322aacfb249dbde04e429df5de57952210f82caf825e93f159' ;; 		x86) natsArch='386'; sha256='4ccf5aa57f33df9591fcce8a1737eb63c71070d09c1a3c098c27865b42803dea' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Mon, 07 Feb 2022 18:40:09 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 07 Feb 2022 18:40:09 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Feb 2022 18:40:11 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd0eec27809c0e4f3462d6b77b4be8cef0024a9e1b10a661198f699c0d031a`  
		Last Modified: Mon, 07 Feb 2022 18:41:02 GMT  
		Size: 6.7 MB (6746426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb62b8bc287d38e4ac6c3c508aaa872195ed1069541208766a12fd2762b7e763`  
		Last Modified: Mon, 07 Feb 2022 18:41:01 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:46214f4467deabc181784961b7819d2d094c1b3c1b9ac2507548d054a5c80200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b9d2149e8e8ea269d90e7002746d2884113c9d938e70b51a419f1b04dde64ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:e0c2e675a7a0aecbe19ab6a7e9fcfba72914e18a89c8f2d82f67a7d5c594631e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fbcee1fbe8fde7a8b3c9ca56b4b60b21610906a11a6f2c5ff4ca9086588dcf3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:d4aec52611b75880c508c2af4f8966af8da75705a444778dab47a33d380c2171
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721197693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8728eebefb79c6df0c72f1c5a104ba76ee51c6e647c48d6079f35b8473f151b8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Mon, 24 Jan 2022 23:18:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 26 Jan 2022 01:15:08 GMT
ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:15:57 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Mon, 07 Feb 2022 19:15:58 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Mon, 07 Feb 2022 19:15:59 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Mon, 07 Feb 2022 19:17:32 GMT
RUN Set-PSDebug -Trace 2
# Mon, 07 Feb 2022 19:19:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Mon, 07 Feb 2022 19:19:28 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:29 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:31 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1e63a09e013659f9cb51a44694cf1487fd0ea2ae5528ca387357386508f2b93c`  
		Last Modified: Tue, 25 Jan 2022 00:07:22 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2d5bbe3c541fe8decf0e3c04bd30aaa74313119e1269d9b03d461638babbd`  
		Last Modified: Wed, 26 Jan 2022 01:19:16 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e72d50e0cde35003b43d8d038e5708f527d97d0a568226eafb301ba849a2b43`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64d29ca5e300bfda3089e1a4884f421acf31b18cdfe01d673e3b90229ed2879`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60b7c6a77eeee69c2e05bc3b0c14b27b306e9ee8f4de5dfd59467ded9c013b`  
		Last Modified: Mon, 07 Feb 2022 19:20:13 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4a43a8e4021d4bd0b12da3c7dcbbe46b75aa546f68d2550c17a7680500219d`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 368.8 KB (368848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639c43c4f3663c8b89b0eb155e796bb8579ba2a1c48ec58d6c2b870997be6fd1`  
		Last Modified: Mon, 07 Feb 2022 19:20:19 GMT  
		Size: 7.5 MB (7496098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6b2aa7fae5dd223e3ef98201acbce49ac6f49520da4b7eacad44e6051d205a`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69816326a205954d2a86794bec6db440cf0012280baaf21ba798f697f59cc081`  
		Last Modified: Mon, 07 Feb 2022 19:20:10 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892fbd0964f5833a503db0d8c64af4ee03159522271e93155f5bc3921b57b38a`  
		Last Modified: Mon, 07 Feb 2022 19:20:11 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
