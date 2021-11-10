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
-	[`nats-streaming:0.23.0`](#nats-streaming0230)
-	[`nats-streaming:0.23.0-alpine`](#nats-streaming0230-alpine)
-	[`nats-streaming:0.23.0-alpine3.14`](#nats-streaming0230-alpine314)
-	[`nats-streaming:0.23.0-linux`](#nats-streaming0230-linux)
-	[`nats-streaming:0.23.0-nanoserver`](#nats-streaming0230-nanoserver)
-	[`nats-streaming:0.23.0-nanoserver-1809`](#nats-streaming0230-nanoserver-1809)
-	[`nats-streaming:0.23.0-scratch`](#nats-streaming0230-scratch)
-	[`nats-streaming:0.23.0-windowsservercore`](#nats-streaming0230-windowsservercore)
-	[`nats-streaming:0.23.0-windowsservercore-1809`](#nats-streaming0230-windowsservercore-1809)
-	[`nats-streaming:0.23.0-windowsservercore-ltsc2016`](#nats-streaming0230-windowsservercore-ltsc2016)
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
$ docker pull nats-streaming@sha256:1686d8fe6667bbf1d7ff4a63ace76c6185008decbcb24e3cd6d188f66379a4f4
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
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine3.14`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-linux`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-scratch`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore`

```console
$ docker pull nats-streaming@sha256:88e97c1278b7a21ba5423e4f27da81a706a9ddd35a4c6f9b609c004cf69009cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:9a930a2436685cc70302853288599a799fc3415f8c20be39f0e05cb522f40ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6872c30a7c75f13ef527c8d3c7411f8438232cb88697fa5f5669c9da884f6157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0`

```console
$ docker pull nats-streaming@sha256:1686d8fe6667bbf1d7ff4a63ace76c6185008decbcb24e3cd6d188f66379a4f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-alpine`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-alpine3.14`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.0-alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-linux`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.0-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.0-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-scratch`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.23.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:88e97c1278b7a21ba5423e4f27da81a706a9ddd35a4c6f9b609c004cf69009cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.0-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:9a930a2436685cc70302853288599a799fc3415f8c20be39f0e05cb522f40ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:0.23.0-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6872c30a7c75f13ef527c8d3c7411f8438232cb88697fa5f5669c9da884f6157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:0.23.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.14`

```console
$ docker pull nats-streaming@sha256:e5649a4a47507b9069440a623bdd5f09a2419bd81debf6e8916e7ab85324895f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.14` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9d1a14ec8294f02ad61859abbae261ed58e52656ca742e506fc959664b834904
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10380582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15d33fcb55af1db00c97fe142efd0d2b9474767a61be57bf2c04f7d245c8e71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 15 Oct 2021 23:32:18 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:32:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 15 Oct 2021 23:32:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 15 Oct 2021 23:32:22 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Oct 2021 23:32:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d98635b1c67ba74edd1c339053b799e81535f34ede771018aa3d1acd660b1b`  
		Last Modified: Fri, 15 Oct 2021 23:33:11 GMT  
		Size: 7.6 MB (7565714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ad9a9bb37a13d2b80423d6893b9217cc45bfc227b6084ac664d6edb1cda628`  
		Last Modified: Fri, 15 Oct 2021 23:33:09 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:94e32218185bce38079a89646554af12973d9c1a66ffc9f423be40fa5e7f5e48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9667646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2a4a22be20ed6a78d3dc32468da4408ee3ad94d70127fb08162e8c8746a554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:09:49 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:09:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:09:55 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:09:55 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:09:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:09:56 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfda0054989a71c89a82b1f380260d3777cc5519f77c1bf34125a4b3463ed9b`  
		Last Modified: Sat, 16 Oct 2021 00:11:39 GMT  
		Size: 7.0 MB (7039777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b9a84c28137138f528f26f1146a1cec8d0a0c5ceb5ab4dc89fe5758c96ec55`  
		Last Modified: Sat, 16 Oct 2021 00:11:34 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b97a1d2f2d3a3be9d6dffa2fd92ff918d307e9f8c7912c7a7bcb323d61ad219b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9464101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74cae53d5fc38e3ae01a55a197956068c56635dde300afb12e3cd17790d0af2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:23:25 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:23:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:23:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:23:32 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:23:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713413651cffbb9013dbcb635cc7d6048e404390ee992d0dc14322b4f31c87ee`  
		Last Modified: Sat, 16 Oct 2021 00:25:15 GMT  
		Size: 7.0 MB (7033258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337725b5b2d314cd44e4554c7cedfe61376e0f0ace7339f343d909eeb9f94f0`  
		Last Modified: Sat, 16 Oct 2021 00:25:11 GMT  
		Size: 424.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c62bf392316ddd25875ed160e0dbd43b3eb58f79e2b216d210959498f48551cf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719e8038a8fa3be083d1e31199895ce43c32a2b70a6f244e8f36b05e0b091d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 00:03:02 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Sat, 16 Oct 2021 00:03:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='997b1235349360c46d37588047f5b1b64e7a8603b84478edf153124f3a0b6fbf' ;; 		armhf) natsArch='arm6'; sha256='127e953a64ba7d88039cf7d688a29f968cadcac2a65e43bf2c93e4055665358f' ;; 		armv7) natsArch='arm7'; sha256='d5f9bf496419f4874c2a10a668d04a858d269aec1b31306e1289ccb12b03217e' ;; 		x86_64) natsArch='amd64'; sha256='4695eca8dbc09c1e363b5e2725eada3a1412a3a71f002ce1208aaab91c03e3d1' ;; 		x86) natsArch='386'; sha256='b6c06a9b1edf69cfa764bc499302d27127212787bbc107045f814ad378eaed49' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 16 Oct 2021 00:03:07 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 16 Oct 2021 00:03:07 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Oct 2021 00:03:09 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9016e5cac797bd165a69dd41ff1d64e5fa2949672aa9281e36d865b6404e0b5d`  
		Last Modified: Sat, 16 Oct 2021 00:03:58 GMT  
		Size: 6.9 MB (6932593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac73239a7164496d5fc076e03bf08e5438d03208201b539b5adf840f49296215`  
		Last Modified: Sat, 16 Oct 2021 00:03:56 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:1686d8fe6667bbf1d7ff4a63ace76c6185008decbcb24e3cd6d188f66379a4f4
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
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:824de21859de835a067753d84de2afca7aaf50d64fa51f02f04abcd494dd7eef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:2dbb43c04baf106a43675bf28777c03264561d3afcdaeb2302ff67cbec5b38af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6750096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e67b7095d95be738308578ecefccfc48eed7b185a9af51b4c28d23b173f67b40`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:23:53 GMT
COPY file:c7dc778964347070ee92c7425dccdc11b1e6461600bba29e95a3b4f6716859d1 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:23:54 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:23:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:23:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2a3880fbf50499b15f6a54fdc688d856d9c4d23cec08a4fd97eed038a214f6ef`  
		Last Modified: Sat, 16 Oct 2021 00:25:47 GMT  
		Size: 6.8 MB (6750096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:88e97c1278b7a21ba5423e4f27da81a706a9ddd35a4c6f9b609c004cf69009cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:9a930a2436685cc70302853288599a799fc3415f8c20be39f0e05cb522f40ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:7027365ba3377b3b4938d7b70075668399e2a43110e2304194caf72766e805ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2714236109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce99330d5b790f9c755844a68ee8f5a54634d1b3a75e4efd7c642457f1de32bf`
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
# Wed, 10 Nov 2021 20:04:14 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:04:15 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:04:17 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:05:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:06:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:06:50 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:06:51 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:06:52 GMT
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
	-	`sha256:6498ab335725fe000ba5144e4d5062ad1975bf67df5dec8246916f4c9bd7f72c`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802da88659bd002452caef70c832d97ec57bd1e8a7c6ea453c5f7ecb7243a8d`  
		Last Modified: Wed, 10 Nov 2021 20:10:13 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f217e07318ca4db5fd7eeced24f90a62438081e2239704e9c9223f746fbfd939`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e92dc31bedbc8373804da8fdc1b5da64c6a16940b3f5c5a0b03baed4a9da40`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 353.3 KB (353303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10c3351bbc8575634f0b1f6771405f07bdf18b95b229ae3eb4baca206756c67`  
		Last Modified: Wed, 10 Nov 2021 20:10:12 GMT  
		Size: 7.8 MB (7750431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cac15efb2e1e79afe1587342933e7af126ee9bfc3d9b068a2be3e15f998fae`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2329e72dad15d4f3b14b52f5c7367ca3ec9d15b3a578105ea5bbc004c7b173cc`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4a22275bb9523c35a263eedfe5757fbcc85c035e7cfdd5d76b0b7589400f0c`  
		Last Modified: Wed, 10 Nov 2021 20:10:10 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:6872c30a7c75f13ef527c8d3c7411f8438232cb88697fa5f5669c9da884f6157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull nats-streaming@sha256:52ce1ef5c3dc6d74602405fb5ffed1443fa8934d2d4f736c5b499c25b7c15349
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285742086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4324dfda0e7b2bbe376cfb195846ac03015ef4a87f43decc5ce2c33a0645cb0`
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
# Wed, 10 Nov 2021 20:07:07 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Wed, 10 Nov 2021 20:07:08 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Wed, 10 Nov 2021 20:07:09 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Wed, 10 Nov 2021 20:07:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Nov 2021 20:09:36 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 10 Nov 2021 20:09:37 GMT
EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:09:38 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:09:38 GMT
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
	-	`sha256:0ec1546ca5a33e6e59ec5fc3841008085ed098a9ea2cdf82c4405b1556f21fe6`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abee19e1083e7b1f34d2539fd8cc45d3f4c5151ecc6071ae85db9f7e83f479ae`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c3353784a0469f6527f18d14abfc00eb4cbeeaec9410cfc9b818839feac8be`  
		Last Modified: Wed, 10 Nov 2021 20:10:40 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a3645203247934dbfb9bcaa7ed260c35ac9776b936d1ea223e501a8a6d791`  
		Last Modified: Wed, 10 Nov 2021 20:10:38 GMT  
		Size: 349.1 KB (349124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f2db37ee09fbb668ce3c50272a21db7121813564213d776c86d38b49bbeb51`  
		Last Modified: Wed, 10 Nov 2021 20:10:41 GMT  
		Size: 12.3 MB (12290794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edadce805210af3798e6823fbbb73cf3268619e2159b65e5c1fd8a5d9572714`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c83b5a63ab16e295cf52b1a22f04d4794fd8a09da5f026e235081de52b9628`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0f820c2bd96784e20f5980017ebfb65b0c4376d18c3e91fdcc2e248de153a0`  
		Last Modified: Wed, 10 Nov 2021 20:10:37 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
