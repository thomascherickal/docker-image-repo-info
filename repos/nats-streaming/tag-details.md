<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.18`](#nats-streaming018)
-	[`nats-streaming:0.18.0`](#nats-streaming0180)
-	[`nats-streaming:0.18.0-alpine`](#nats-streaming0180-alpine)
-	[`nats-streaming:0.18.0-alpine3.12`](#nats-streaming0180-alpine312)
-	[`nats-streaming:0.18.0-linux`](#nats-streaming0180-linux)
-	[`nats-streaming:0.18.0-nanoserver`](#nats-streaming0180-nanoserver)
-	[`nats-streaming:0.18.0-nanoserver-1809`](#nats-streaming0180-nanoserver-1809)
-	[`nats-streaming:0.18.0-scratch`](#nats-streaming0180-scratch)
-	[`nats-streaming:0.18.0-windowsservercore`](#nats-streaming0180-windowsservercore)
-	[`nats-streaming:0.18.0-windowsservercore-1809`](#nats-streaming0180-windowsservercore-1809)
-	[`nats-streaming:0.18.0-windowsservercore-ltsc2016`](#nats-streaming0180-windowsservercore-ltsc2016)
-	[`nats-streaming:0.18-alpine`](#nats-streaming018-alpine)
-	[`nats-streaming:0.18-alpine3.12`](#nats-streaming018-alpine312)
-	[`nats-streaming:0.18-linux`](#nats-streaming018-linux)
-	[`nats-streaming:0.18-nanoserver`](#nats-streaming018-nanoserver)
-	[`nats-streaming:0.18-nanoserver-1809`](#nats-streaming018-nanoserver-1809)
-	[`nats-streaming:0.18-scratch`](#nats-streaming018-scratch)
-	[`nats-streaming:0.18-windowsservercore`](#nats-streaming018-windowsservercore)
-	[`nats-streaming:0.18-windowsservercore-1809`](#nats-streaming018-windowsservercore-1809)
-	[`nats-streaming:0.18-windowsservercore-ltsc2016`](#nats-streaming018-windowsservercore-ltsc2016)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.12`](#nats-streamingalpine312)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)
-	[`nats-streaming:windowsservercore-ltsc2016`](#nats-streamingwindowsservercore-ltsc2016)

## `nats-streaming:0.18`

```console
$ docker pull nats-streaming@sha256:381b124fad3569937d92c6aa1caa775b508584cbd05c2c40e3c7189772b15f08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0`

```console
$ docker pull nats-streaming@sha256:381b124fad3569937d92c6aa1caa775b508584cbd05c2c40e3c7189772b15f08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-alpine`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18.0-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-linux`

```console
$ docker pull nats-streaming@sha256:f346ed12fc02e108b0c713aed44239ec6e6b7ea6a3dbbeb58f5390f4b337f14b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18.0-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18.0-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-scratch`

```console
$ docker pull nats-streaming@sha256:f346ed12fc02e108b0c713aed44239ec6e6b7ea6a3dbbeb58f5390f4b337f14b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a3cf18102bec632be2795c497e01477397d754cf29d6a8f71f4b28e99f209c05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18.0-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c3bc4f1f972dc1f5ef1df2d337acb58dc3ef8789bf4a3b4a9b433e1177da1380
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18.0-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:54d40e51d875bc81bb945b41864cd2ec42895f68ec32ec2f381fbe16aa91dd2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:0.18.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-alpine`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-alpine3.12`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18-alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-linux`

```console
$ docker pull nats-streaming@sha256:f346ed12fc02e108b0c713aed44239ec6e6b7ea6a3dbbeb58f5390f4b337f14b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-nanoserver`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-scratch`

```console
$ docker pull nats-streaming@sha256:f346ed12fc02e108b0c713aed44239ec6e6b7ea6a3dbbeb58f5390f4b337f14b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:0.18-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a3cf18102bec632be2795c497e01477397d754cf29d6a8f71f4b28e99f209c05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.18-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c3bc4f1f972dc1f5ef1df2d337acb58dc3ef8789bf4a3b4a9b433e1177da1380
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:0.18-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.18-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:54d40e51d875bc81bb945b41864cd2ec42895f68ec32ec2f381fbe16aa91dd2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:eff8ac1f5a7e6729103dfcc46da04d450d64b0145b214ab4b6c7b6158b6a63fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:9f71614879c6e9c774410e5315004fc3f6b8f2e52a6e1c6dbe2f203e6c285df0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9015136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5b225e159253af34dce2a69079773d857596bf528268a384b2fd1a0b8af6f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:25:24 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:25:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:25:26 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:25:26 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:25:26 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638813c8986e4931f6582e649523542695f342c8cb8083284a6c1e1cd7b4b119`  
		Last Modified: Thu, 25 Jun 2020 19:25:59 GMT  
		Size: 6.2 MB (6217173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba66f363cd2d1a64d4578d0f9f604c52be7e910debc173b3c61aef5549ed716`  
		Last Modified: Thu, 25 Jun 2020 19:25:58 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5e26f04be49fde97b89ffbe97802d111bb613022d4157384f8dff1f965353233
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8414429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0081104aa8b1b99cca0a885d70e36b87da9f8b46e2680f818f427c3aff3db082`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 19:50:21 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 19:50:29 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 19:50:30 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 19:50:31 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea42d87d9aceed297b04cbb66a98d0502d1a4e4d7fbf4a24da0eb5e117aa0b34`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 5.8 MB (5810721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ee71ef2c48adc42b0180ed8f9f18ec21b79821006b92b9c101969c91ca0cd`  
		Last Modified: Thu, 25 Jun 2020 19:51:05 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:edc847c0db6be8390fb0d380f79011c2b9a250c2fd8127dc42c7fb46ccfa2162
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8213838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc8a653819ac1d586c5211f81be29e3376947f8eb669460a290893d6daa4ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 25 Jun 2020 18:58:53 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 18:58:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		arm64) natsArch='arm64'; sha256='ff2a51618b79685264f980fe868f1c7af583c419b6406cc63d4811f3c98ca8fe' ;; 		armhf) natsArch='arm6'; sha256='629e17255f12fd80e051772a6dd18a7f65e692b4abef0786b421eb8b6ab85db4' ;; 		armv7) natsArch='arm7'; sha256='94e499af6a6391519315e8bcd5127c43c1d1a442ef945956286e77b4366c92c9' ;; 		x86_64) natsArch='amd64'; sha256='6252e9262efc81a41ade3f43b68e014d1e635d3e3bf9cbcd2b09c3a030a0d5e6' ;; 		x86) natsArch='386'; sha256='886ebd2e5eb99e30ff9e9d8907d7bd49dafacffce1dc921427e5754a4ec26f55' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Jun 2020 18:58:58 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 25 Jun 2020 18:58:58 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 18:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Jun 2020 18:58:59 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286fedac0aa1b93bebceb6fbb3de07a7c57160e1fd714403afea49b08e2887ce`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 5.8 MB (5806653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f45eb729be07e4f3dffb7b479060f228cab76029542a382f3d9d661cde0a0c5`  
		Last Modified: Thu, 25 Jun 2020 19:03:10 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:ce0701d5e502d2a1c4d19740c2ce406b988afee6b45d0a6edba1687e0df7b644
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:d51446476985b28e3adbe2fade2829a4422cc9772a381102d6d028c692f6103a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5532577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66abc9c11dbf79a012e2eb7942c925497ec745126c3c0fa84b0f6f9c802d2aac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Feb 2020 20:55:22 GMT
COPY file:fe34ad03c894e889c935d94d7e07558f20273a5d297c14329deebd7179819ef8 in /nats-streaming-server 
# Tue, 11 Feb 2020 20:55:23 GMT
EXPOSE 4222 8222
# Tue, 11 Feb 2020 20:55:23 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Feb 2020 20:55:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5e82baaeaf291facb7d5f2b85f4a96bda41038775d2a804a293d31701833d65f`  
		Last Modified: Tue, 11 Feb 2020 20:55:36 GMT  
		Size: 5.5 MB (5532577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:324fd9f26319ea86c85d18b877b5815252be2deeb96da86f73d74b6e8b887695
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:d51446476985b28e3adbe2fade2829a4422cc9772a381102d6d028c692f6103a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5532577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66abc9c11dbf79a012e2eb7942c925497ec745126c3c0fa84b0f6f9c802d2aac`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Feb 2020 20:55:22 GMT
COPY file:fe34ad03c894e889c935d94d7e07558f20273a5d297c14329deebd7179819ef8 in /nats-streaming-server 
# Tue, 11 Feb 2020 20:55:23 GMT
EXPOSE 4222 8222
# Tue, 11 Feb 2020 20:55:23 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Feb 2020 20:55:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:5e82baaeaf291facb7d5f2b85f4a96bda41038775d2a804a293d31701833d65f`  
		Last Modified: Tue, 11 Feb 2020 20:55:36 GMT  
		Size: 5.5 MB (5532577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:6f44767248a033de66eeec67cb01c305c3557412bf7785fed59732b15b4d51d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:2d364061b4734fff31048f41a5fad0201aa297599fa4d31dae05cb8d1cda1116
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.0 MB (106991103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b303f1177c01c28fd06a91ab80e797e1405e9caaa38a2d9828ba723db365035`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Wed, 10 Jun 2020 16:04:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:45 GMT
RUN cmd /S /C #(nop) COPY file:4a858ac4da943f868519572e3fb6817fd379875f2bff0bcb5f03c5bdddc496a8 in C:\nats-streaming-server.exe 
# Thu, 25 Jun 2020 19:16:48 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:49 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fd97aa6008f57e8475bff231216617c39835f885adb6a9c73a3a1599e2d788b9`  
		Last Modified: Wed, 10 Jun 2020 16:08:53 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20f79cf6dee5a5c8a52b6fb88ca9699cb2f31944f8fad85542d4716c2dbb8f`  
		Last Modified: Thu, 25 Jun 2020 19:20:46 GMT  
		Size: 5.9 MB (5944129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc82a844c5312714697a55298674c4a5c5ee1b7baeece61d8e06c9ed4e50ea60`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 911.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a2429531df489d0d6c5f806f036470f4ff64eaafda28a8178f0fc85a58e58`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa9cbf8170aee07fe7c29ddd0abb740a16d0cad5a552f262d22f722b23ab511`  
		Last Modified: Thu, 25 Jun 2020 19:20:44 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:f346ed12fc02e108b0c713aed44239ec6e6b7ea6a3dbbeb58f5390f4b337f14b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:95ded92d384b4d9631841677a2d34b175cba6cbb4b4fa127b7a754b9f57c849e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5530521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24577fc60833cbc345883a4b8ee0eed5044ed08c199307ea0b9f951f7d5b6d3c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:50:40 GMT
COPY file:7145d006cd221687dcd9139e9e58f09c1f07ee9ce00f3485d297197fdd5ba444 in /nats-streaming-server 
# Thu, 25 Jun 2020 19:50:41 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:50:42 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:50:43 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ef961e603a1ec489ef1932fb068478ad9e98f8417ff4fefb8d4678e8653a5771`  
		Last Modified: Thu, 25 Jun 2020 19:51:16 GMT  
		Size: 5.5 MB (5530521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:60e9dc71017275b017a750e7be04e9c16abd50c6b6bc589ddf399588e44a509c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5523586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b24c4ac594ac46c22186488b6b2138f48703c79ebce756ae461ac777a7b486`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:02:38 GMT
COPY file:2b6e0add99a6d3c42ba8b65af53581560646dbdaf347b23e6dde1f4267fa57bc in /nats-streaming-server 
# Thu, 25 Jun 2020 19:02:38 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:02:39 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:02:40 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7af54707b9f6fd805487c0afe7fd52962e5abd3d1ab43335ccfc7224a2018844`  
		Last Modified: Thu, 25 Jun 2020 19:03:22 GMT  
		Size: 5.5 MB (5523586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:a3cf18102bec632be2795c497e01477397d754cf29d6a8f71f4b28e99f209c05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:c3bc4f1f972dc1f5ef1df2d337acb58dc3ef8789bf4a3b4a9b433e1177da1380
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull nats-streaming@sha256:fccf91ec6703587be4343172ce28aafedeaa70a0e124e6e6692a423165fa1b8a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2309404710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133672bcd5cfbbacf6b0a64ea13bc17159ad634ba3a26595d3d070ab81a4c31`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Jun 2020 01:48:42 GMT
RUN Install update 1809-amd64
# Wed, 10 Jun 2020 12:43:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:02:03 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:14:32 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:14:33 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:14:34 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:15:08 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:16:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:16:24 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:16:25 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:16:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:666079ee04606f07f4a27dd98526f5049ef8fed93e347d8b4c447b0d5060c77d`  
		Size: 575.6 MB (575581379 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b11029314f3c794dc51e43c915b3e62f6b44aeb96f84b8b92f453e61cf7a2cb3`  
		Last Modified: Wed, 10 Jun 2020 15:34:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2192add29c9167423d378daa499903c4488337cdc2cf961ebeb0e4c0b492f9`  
		Last Modified: Wed, 10 Jun 2020 16:08:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdc3ac2d9ccd0382babff697996c03e73078cea8cd708ae249f9f7e440a495a`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08db7f0f23bcbaf120f7ce31d3b645acbd51ec9ec2b9c5f0de02713ce1a20846`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a14a4e817fcb29d1f6c15cfe682270eab5b418e5368ab5d33d98b941e580c41`  
		Last Modified: Thu, 25 Jun 2020 19:20:28 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be6a9189710ce278b6d6e9e49b49ff0891d78bdd64ebfb2c5a2c36dd987fc95`  
		Last Modified: Thu, 25 Jun 2020 19:20:27 GMT  
		Size: 4.8 MB (4787569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a8c2acc0287c3ef79dd6c22afecade9ed9deaa5295912427651209679dfd6`  
		Last Modified: Thu, 25 Jun 2020 19:20:29 GMT  
		Size: 10.7 MB (10693762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a914cfe5af6c345eaa54dfdcfc9774913b1f1c9f5a10a74b50941305a0bfa454`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7235d4bb5ccdbdcf9eed6b2d280b46d296002871faa1fb4d2bd21e90cce7a48`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca308b080197d582de4106f74424ad989679cbd06b09832c832607a3776d5411`  
		Last Modified: Thu, 25 Jun 2020 19:20:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:54d40e51d875bc81bb945b41864cd2ec42895f68ec32ec2f381fbe16aa91dd2e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:1114f61e45775a36a2bbfa0b3404c65f9c57ee01c48de00cb7c7295fdc8eb88e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5755256249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c3dc35de6edc22e58f63b69b5b54363526d18f429fb85b27f37bc15c32ae04`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 12:52:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Jun 2020 16:04:27 GMT
ENV NATS_DOCKERIZED=1
# Thu, 25 Jun 2020 19:16:55 GMT
ENV NATS_STREAMING_SERVER=0.18.0
# Thu, 25 Jun 2020 19:16:56 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.18.0/nats-streaming-server-v0.18.0-windows-amd64.zip
# Thu, 25 Jun 2020 19:16:57 GMT
ENV GIT_DOWNLOAD_SHA256=a0c0261df2ce589fe9706617323e06c5bcae70511112eae921681b1169674bc8
# Thu, 25 Jun 2020 19:18:01 GMT
RUN Set-PSDebug -Trace 2
# Thu, 25 Jun 2020 19:19:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 25 Jun 2020 19:19:59 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:20:00 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 25 Jun 2020 19:20:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30efe9163d37226b077b25cd93b088cebd2ddbaadf173d143b9fe0ddecaeae53`  
		Last Modified: Wed, 10 Jun 2020 15:34:41 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f945dc3cc7d024d3f86a74f177545b57d99c3209592a625bb655bf01921d2c`  
		Last Modified: Wed, 10 Jun 2020 16:09:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3713b83b4c75d0a80e8687bc45df0c5bd354e620902411ad1b3028c9dceb2bf5`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c381803b95a9448680f1e9ff9ef8386e9acd31f7481b2a2035b3465d15cf25`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8435805852c6bcef95774603f6342eee8cb5011e45e0df4bd6748a44a16a69e9`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf82c782533604d6df3b87130cef3e947dadecf3e6901038e69bdcc42d1432c9`  
		Last Modified: Thu, 25 Jun 2020 19:21:02 GMT  
		Size: 5.4 MB (5391316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23a41a97ee171205d62ebd2014d3048882dee3fadd09cdb07b4aaf2bdf4ff94`  
		Last Modified: Thu, 25 Jun 2020 19:21:03 GMT  
		Size: 15.9 MB (15858190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373353a28d2cec1c03404ca3f978e36be91bd0101fc6833d413336688c879d1f`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8695528b591a7419d30570a035a97b0a041ad7951e26210e29b1236b61f86d04`  
		Last Modified: Thu, 25 Jun 2020 19:20:59 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6562c9c2a1ce35eb664d14dcf45dab39154e7954e54029ddf893b339a7e0df5`  
		Last Modified: Thu, 25 Jun 2020 19:21:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
