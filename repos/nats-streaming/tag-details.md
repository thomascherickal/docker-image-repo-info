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
-	[`nats-streaming:0.24.0`](#nats-streaming0240)
-	[`nats-streaming:0.24.0-alpine`](#nats-streaming0240-alpine)
-	[`nats-streaming:0.24.0-alpine3.15`](#nats-streaming0240-alpine315)
-	[`nats-streaming:0.24.0-linux`](#nats-streaming0240-linux)
-	[`nats-streaming:0.24.0-nanoserver`](#nats-streaming0240-nanoserver)
-	[`nats-streaming:0.24.0-nanoserver-1809`](#nats-streaming0240-nanoserver-1809)
-	[`nats-streaming:0.24.0-scratch`](#nats-streaming0240-scratch)
-	[`nats-streaming:0.24.0-windowsservercore`](#nats-streaming0240-windowsservercore)
-	[`nats-streaming:0.24.0-windowsservercore-1809`](#nats-streaming0240-windowsservercore-1809)
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
$ docker pull nats-streaming@sha256:26c66c4580815793025369e1432fc9514894703a1d7725fe8cd522361ffbb13c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine`

```console
$ docker pull nats-streaming@sha256:b98abe78a95e9e177052f9f6368aa103148334b2555c3cdacf0582b6d22e3f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:b98abe78a95e9e177052f9f6368aa103148334b2555c3cdacf0582b6d22e3f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:55069c45176b4a75dfb18c462fabcaa61556f5e9853c58762e76e618e9424d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-scratch`

```console
$ docker pull nats-streaming@sha256:55069c45176b4a75dfb18c462fabcaa61556f5e9853c58762e76e618e9424d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0`

```console
$ docker pull nats-streaming@sha256:26c66c4580815793025369e1432fc9514894703a1d7725fe8cd522361ffbb13c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-alpine`

```console
$ docker pull nats-streaming@sha256:b98abe78a95e9e177052f9f6368aa103148334b2555c3cdacf0582b6d22e3f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-alpine3.15`

```console
$ docker pull nats-streaming@sha256:b98abe78a95e9e177052f9f6368aa103148334b2555c3cdacf0582b6d22e3f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24.0-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-linux`

```console
$ docker pull nats-streaming@sha256:55069c45176b4a75dfb18c462fabcaa61556f5e9853c58762e76e618e9424d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-scratch`

```console
$ docker pull nats-streaming@sha256:55069c45176b4a75dfb18c462fabcaa61556f5e9853c58762e76e618e9424d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:0.24.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:ee1a015a6b5d4144fbfc8b436c0f0e79b86562b3d10afed92662c62573c36851
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:33d7a075703135ba18cf4918fccc35e6fbef1f74ac8bb18abb89a62fde7c4e02
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10404541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0d37898667fe6fa6289417167d7e7ce3799d21b08dc0ea4276850e2e8b54b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:20:53 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:20:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:20:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:20:56 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:20:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b719fc3addd4e8cc595271456fe9f9de32955502a0f0cadd27a40bfdce67cdf9`  
		Last Modified: Sat, 20 Nov 2021 02:21:41 GMT  
		Size: 7.6 MB (7581138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae16eed54939fd32b16d2ffcc1ac1e816da3a11b3656bf2344d9d3180173bf5`  
		Last Modified: Sat, 20 Nov 2021 02:21:39 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:8d102ba94dd539c86ae564d1671562cd9687b6001ef28c0a3b9358a31b395259
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9487244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe704390d0d6f143b4d58b95fdb72ffd4050dc343669fad7792a25bbd8fc6ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 02:33:41 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 02:33:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 02:33:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 02:33:47 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:33:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 02:33:47 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b93296bc34cee4aad9d52835eae7e820697f4e8ce382165efb96a8901ea0c`  
		Last Modified: Sat, 20 Nov 2021 02:35:32 GMT  
		Size: 7.0 MB (7048204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c793edf6a99d693922586d1182b7f23998316f40d7f5f9e9c74fca0561094`  
		Last Modified: Sat, 20 Nov 2021 02:35:27 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:c87eb1e5ff911b6ca53a44595f294a4e79baef015629cd41355e25a3bcbebffc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9669856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89205df0bff2640b3f02b3d8eddbce0582d123a8e34ae55fa68fb034b4e42bb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 20 Nov 2021 04:20:45 GMT
ENV NATS_STREAMING_SERVER=0.23.2
# Sat, 20 Nov 2021 04:20:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='623cd04855e16ca52694964e01e3b50ded9747a45885bba1a705513da297f6fd' ;; 		armhf) natsArch='arm6'; sha256='fd40f251da335eb7b3cc63b08f8bc0a80d3a4df10fec4efdf6e60417248a5287' ;; 		armv7) natsArch='arm7'; sha256='83db867570654731de98f135f9f373d0758bd9c5a3ee304b65c8128e1d928023' ;; 		x86_64) natsArch='amd64'; sha256='d0c5ebc16901bdc4788d0382dab6f7ce69582e1bafea3ddba159b38ae87b6c81' ;; 		x86) natsArch='386'; sha256='8b9c5396a7747abc8415dc8ca915cf6cb2fd1b79b64ce7a4c3f5efb241cd389f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 20 Nov 2021 04:20:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 20 Nov 2021 04:20:50 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 20 Nov 2021 04:20:52 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a942eeaa58bb70c5a728104921dad38ccc6d39aca7c779aa1431c751506e6ab`  
		Last Modified: Sat, 20 Nov 2021 04:21:41 GMT  
		Size: 7.0 MB (6951735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd89828a2f02db651c46db6cbf2f637d36ecc30f847933336bb73135367cd013`  
		Last Modified: Sat, 20 Nov 2021 04:21:40 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:b98abe78a95e9e177052f9f6368aa103148334b2555c3cdacf0582b6d22e3f25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats-streaming:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:5d5fa97b46fc4ca4014ba25d9ddf70b80a038c040c2a465c4d484a71ba08d1c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9463324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ee3f9a30b7d12feb0a7b3bdedfd6339f86f655bd9f5df78a7a062c8fe49892`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 00:55:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 00:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 00:55:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 00:55:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 00:55:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89b8a8ca7bbb99f912eda88195a5d7ff13d719967c443f18a8b6c1fcc5fcf7`  
		Last Modified: Thu, 27 Jan 2022 00:57:16 GMT  
		Size: 6.8 MB (6831480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec34e193ec327fe40cab042da1d4b25023daf509bd2949069454d5572bd7b1d`  
		Last Modified: Thu, 27 Jan 2022 00:57:12 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:af08f1a8fcf45d5c047765faae58e6371583868accc47db94bca333a3b58e04d
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
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:2634d6d948732eb88bc617d6cdc2fded0effe0eec6bdb0e7e4c274bea30eebe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ea0466ff603970b10676172d9848be558dbad12d415017f97a961b7e0f7b0f20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:899f57d6f57b29694ca96bb793f8c75b6bc29991fba14552b3f6c4049813de09
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110202498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dace8e030565c6bdece22fe59259ea5d049129ec0061453d8eb7992742c94d9`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 27 Jan 2022 01:17:36 GMT
RUN cmd /S /C #(nop) COPY file:109deef90b885a26302b64839c78333783e58da8dd23f89e7162f625883f0aa0 in C:\nats-streaming-server.exe 
# Thu, 27 Jan 2022 01:17:38 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:39 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:40 GMT
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
	-	`sha256:c8612b227ef0df818228cb4aabbe9fc07e04131d539e005fe90ef2119a079b92`  
		Last Modified: Thu, 27 Jan 2022 01:18:26 GMT  
		Size: 7.2 MB (7151318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da34468060e4859dfea2c77ea6e57a35dde56ecb758644158ecc34865471cc5`  
		Last Modified: Thu, 27 Jan 2022 01:18:23 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741461a2bbff23d001731f3cdc69ff196d5bbb7f536f05682db3beea226df491`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f210f52731e0ca9b879df279bba4a22b9f9c789132cb521e61c079ca63892f`  
		Last Modified: Thu, 27 Jan 2022 01:18:22 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:2634d6d948732eb88bc617d6cdc2fded0effe0eec6bdb0e7e4c274bea30eebe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:05a387b6bd267efd7806a67b7b4d431d054e69537a8dd00f0a874e71b48be7e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7299150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1cf392bf11cb1f2dac51f4d09fa86f69859583c3ac7d4812f6c1887d485073`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:21:16 GMT
COPY file:430b600f51b8ec2b8032b9ee2b54a3f23458b67e7fcd26e03d4a1c4fb292e8e3 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:21:16 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:21:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:21:17 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ea39d064fdb9df476b776a2728cf769791a02b09590387975647243e2266b1ca`  
		Last Modified: Sat, 20 Nov 2021 02:22:01 GMT  
		Size: 7.3 MB (7299150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:70edae45d21ebba44c24fb1c18f3192158d7e00ed2c4af215d45477a72463994
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6558012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694806db44c422954ff476d7eb07a53b5b7ebd04177699afaa53a4f525842e07`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 00:55:51 GMT
COPY file:b1726d9c592d47fd10b019c5be7309fe30f8c1b8fee7cad066ae205324061c96 in /nats-streaming-server 
# Thu, 27 Jan 2022 00:55:51 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 00:55:52 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 00:55:52 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4d610c82a45aa47531bfb809dc3656603559a8bfa3d5b53480c8d2659b7c977b`  
		Last Modified: Thu, 27 Jan 2022 00:58:09 GMT  
		Size: 6.6 MB (6558012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:cf7abf017ca4b10bcc16492ee29f54f9901fc6c40ae0e5eeba35423ce4346312
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2b939f92968d68a30b61db2b05fae78f9b7545fb1060ebb0c535069d2a6e0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 02:34:09 GMT
COPY file:f737534371c307ebba33d860a23821186a07bfe6bac93b4f8db1052afabca519 in /nats-streaming-server 
# Sat, 20 Nov 2021 02:34:09 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 02:34:10 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 02:34:10 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:f09d0d006743cce0f69db665ba3e97775e3e7ec87b782222a87b0e299de7abdd`  
		Last Modified: Sat, 20 Nov 2021 02:36:04 GMT  
		Size: 6.8 MB (6763075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:62364f60027f7c3607653a956cf2578021f20431d07038537298bd2e053f622d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6666709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e200b7f1afcc145455136db22812cb59ac4b91d3018f34d80f3df1980798dfa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 20 Nov 2021 04:21:01 GMT
COPY file:758facc101ea28c799c8630223bb78d0e4182d429b666642665350bc7a40a28d in /nats-streaming-server 
# Sat, 20 Nov 2021 04:21:01 GMT
EXPOSE 4222 8222
# Sat, 20 Nov 2021 04:21:02 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 20 Nov 2021 04:21:03 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:372c129ce02fe71df79c38000ee3af5425ca18626def1095c58ab7c9cc6a31a8`  
		Last Modified: Sat, 20 Nov 2021 04:22:04 GMT  
		Size: 6.7 MB (6666709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:00d8d77387fabe6ce44fa62d1e20878940ed98752c954936260476241bc1e2b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:5e291bab0c4e5bd93ee4469028b60d41679f10671cb979788c67bf8332de690f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721195641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba96c680bc990d9ad17e9232df39dec619634c92eb3581031dd578af41b90d8`
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
# Thu, 27 Jan 2022 01:14:08 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 01:14:09 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.0/nats-streaming-server-v0.24.0-windows-amd64.zip
# Thu, 27 Jan 2022 01:14:11 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8c8a8e54d31aa858d687d7e50eb467597e9a613747d7a9cbe3d0e0b1f70cca57
# Thu, 27 Jan 2022 01:15:17 GMT
RUN Set-PSDebug -Trace 2
# Thu, 27 Jan 2022 01:17:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Thu, 27 Jan 2022 01:17:20 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 01:17:22 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 27 Jan 2022 01:17:23 GMT
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
	-	`sha256:53a88cc6db0bc80552df9bfb113308c04aa1ec0a3b3890d7ab65ff01c9ee616b`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2289dd018be6a0a4cdba1897381b2e84b55510c892474da492079b1bec0ab760`  
		Last Modified: Thu, 27 Jan 2022 01:18:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c006d1c5289702608f08f5c9f6a9de93d95ad3d221c0a428a051bb08853314f1`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ceecdae2aa200856facae4f882cccdec07c5f73fa6be67102a25e9cc59b33d`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 368.5 KB (368481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda1285a23cc1cddd740a74ef262ce38497a96b2c2e1b6a6590b54a0e7927daf`  
		Last Modified: Thu, 27 Jan 2022 01:18:09 GMT  
		Size: 7.5 MB (7494276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3379738b94b87894e4d2daf05a77f9e18d4e5bf53cd3ab68d91f44909089c1`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ca9dece730bdc0d6aa28750048d7884f5bc7a5a28b5fee45cbad75bb5ceaef`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0df19e03f80b2c1159d6075d4e03d8fe4e35d0500ddee3812f96398160aad8`  
		Last Modified: Thu, 27 Jan 2022 01:18:07 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
