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
$ docker pull nats-streaming@sha256:2f0606dfe0d7fb28b732e022cd691fd3155e72b8245675c349a688d4134569a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

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

### `nats-streaming:0.24` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1`

```console
$ docker pull nats-streaming@sha256:2f0606dfe0d7fb28b732e022cd691fd3155e72b8245675c349a688d4134569a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

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

### `nats-streaming:0.24.1` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24.1-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24.1-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24.1-windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.1-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:0.24.1-windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
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
$ docker pull nats-streaming@sha256:2f0606dfe0d7fb28b732e022cd691fd3155e72b8245675c349a688d4134569a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

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

### `nats-streaming:latest` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:708884945e9412670acbefb3f8de5f34ea2e6f8053398f3c692e6ec325e8b271
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:4e8a61610850ff6bb549dd019fcbcdc13573bf1ccc9a208d1ce4615e794bf6da
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110244406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a49d85b84f5654522649cf3f61c8d41af27b4a37a83b6d5d396b48e52d793bbd`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:13:38 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Wed, 09 Feb 2022 18:13:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:41 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22ae2eb4723d82be46a897b6eb8b20ac31dc237439701d655c36d80f4c5e6e`  
		Last Modified: Wed, 09 Feb 2022 18:14:29 GMT  
		Size: 7.2 MB (7152685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc984d9f102502f8bdc0fb6105e87b7dbc8a2897ad41d31e3e819cd801719a03`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bfcbb4253358244634febb61fb3145c20ac24af528164ae8a1b00489859a70`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4e6512326439db0b43fb7fe412e40cf42832e75dadcdb785925c91d8dc6dab`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.2 KB (1161 bytes)  
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
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:b8fd3159fa671daeead015b6714594225243e808ed9c7dc0b2ac33c70d0cb3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats-streaming@sha256:f312e17cc06ecd7a585d7a4efb239c96201bf492a98a2513165b66e5a5498d67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721556721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b5f3a39e13fecd674f6808c4ee78017ad62dad829fbc8c7ab8f9d923fcd8867`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 02 Feb 2022 19:28:56 GMT
RUN Install update 1809-amd64
# Wed, 09 Feb 2022 15:04:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Feb 2022 18:10:54 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Feb 2022 18:10:55 GMT
ENV NATS_STREAMING_SERVER=0.24.1
# Wed, 09 Feb 2022 18:10:57 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.1/nats-streaming-server-v0.24.1-windows-amd64.zip
# Wed, 09 Feb 2022 18:10:58 GMT
ENV NATS_STREAMING_SERVER_SHASUM=40fa6c1f7a820c06ff8bec759270e1e30d295021c49bf8aafd67651f89cd84e7
# Wed, 09 Feb 2022 18:11:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Feb 2022 18:13:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Feb 2022 18:13:24 GMT
EXPOSE 4222 8222
# Wed, 09 Feb 2022 18:13:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Feb 2022 18:13:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1bd78008c728d8f9e56dc2093e6eb55f0f0b1aa96e5d0c7ccc830c5f60876cdf`  
		Size: 995.4 MB (995381853 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49d3791198cf2ea875fd54ce3bb715670742d4a58c00252395ad1b74036662a`  
		Last Modified: Wed, 09 Feb 2022 16:39:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4235aeeb4e8b577cc7aa26c7994ec94c94dd53a38764fc510b330b77cef4abad`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2261f128322c729f753da9516033f8d788e9ca448947816ca4eb0415c716e54f`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e13dee75beaec489ba79e703f872b35c086ef77445198b937afbe7678b747`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae753cc9850c82671c1189b2524659b7d452a6abb8ef0870257e71150349ae9`  
		Last Modified: Wed, 09 Feb 2022 18:14:09 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dbfe03a29f9113312e493b332728cf2f38053dcf0af88593c6d9c7db1380`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 351.8 KB (351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4ce59ba4bf0bc375c6e81604a4dfebfa88b0d0bece776f101f46d3bf54de44`  
		Last Modified: Wed, 09 Feb 2022 18:14:15 GMT  
		Size: 7.5 MB (7478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23041a9d1396e9aac1572d5b165ef06ca0f08e61e2b5543eedb20e9c97c87d7d`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b13f5156d1f0b0b1d12513f662a40c9ff550373e9ec00a353b3fac7d0bb2a`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44064770ef00350dbefc6557f0cd98dca0281cead175d42e3b9df48fd1d2fb4e`  
		Last Modified: Wed, 09 Feb 2022 18:14:07 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
