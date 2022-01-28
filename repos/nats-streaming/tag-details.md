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
$ docker pull nats-streaming@sha256:fa0f8012a8ceeac28c9807c4cbc45134c9f690968a23742ceca3c631cb971c00
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
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:fa0f8012a8ceeac28c9807c4cbc45134c9f690968a23742ceca3c631cb971c00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:0.24.0` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24.0` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.0-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24.0-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-alpine3.15`

```console
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.0-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24.0-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.0-linux`

```console
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.0-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24.0-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24.0-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:0.24.0-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
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
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:70806391edbb4a25bffabd5e73b4ccd2411dfbd3a49765b244c7ab595bccfae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fcd566240a0d3fcbd2c974d34a59de00c81f5f666aacb04879966c3b67667476
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10132072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e040cce22c489471df3a493aacea018989603acfb447d3ae151b873960c9e68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 23:28:28 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 23:28:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 23:28:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 23:28:31 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 23:28:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d42a944988bdc9c72ea7d06073b1bcde367b7c4d5f60ad8d683bbc44252d1e`  
		Last Modified: Thu, 27 Jan 2022 23:29:44 GMT  
		Size: 7.3 MB (7313237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d8a0a864a21d26d58490e86ae25681a478ae5f4816b36b342596ffcb748c0e`  
		Last Modified: Thu, 27 Jan 2022 23:29:42 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `nats-streaming:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:1a40f0bbb71636984d1ef88c85c3be3abfe1e687f99d207a8347666b69ee3552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9256569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cddbc61c5eac6bac877e61d2be7f199b2b9f4e885a6c69ca905129e2f769629`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Fri, 28 Jan 2022 10:47:11 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Fri, 28 Jan 2022 10:47:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 28 Jan 2022 10:47:16 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 28 Jan 2022 10:47:16 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jan 2022 10:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37f9531b4294af58f24be77aafdcb7903f3a2605f77c1b0c7d632b4705598b7`  
		Last Modified: Fri, 28 Jan 2022 10:49:09 GMT  
		Size: 6.8 MB (6821382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80303ce3c6efd666406aa68c2a322404cea9fce7d1601393ee190164407d32d9`  
		Last Modified: Fri, 28 Jan 2022 10:49:05 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:28ca65a58fd65967772aa931050e2837907329dadd8ddb9458214fa84b0ba452
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9458812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4d69abd8b3fd92d8a726de49c3df4bcdff19dbe21db8dd4d5e8c22b2f88dab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Thu, 27 Jan 2022 05:48:26 GMT
ENV NATS_STREAMING_SERVER=0.24.0
# Thu, 27 Jan 2022 05:48:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='30cfc19cbc65437a0766c0660433282c410e013500bd27eef8c642f2edccce39' ;; 		armhf) natsArch='arm6'; sha256='c9a2df743ff09b2cb69ebce3f83c5ea8b62dfff7c64590445f4762633e9d8b70' ;; 		armv7) natsArch='arm7'; sha256='ebebef3f5be432dbfeb691e21f4752d153c00b5323d1ecd41b485ee4582fb7c9' ;; 		x86_64) natsArch='amd64'; sha256='c0be4d653df64ba698a747c1a255808c993226f1e703fc309c4a35a74e491cd6' ;; 		x86) natsArch='386'; sha256='27bcb3cde323f5b1e1e56bb09a97c4290ff71df7f5343ac8ad994c3335f24c29' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 27 Jan 2022 05:48:30 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 27 Jan 2022 05:48:30 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 05:48:32 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5466655b4ebbac1a6e295f91817671e93c5c08ea95df05f263da81c752aa4397`  
		Last Modified: Thu, 27 Jan 2022 05:49:34 GMT  
		Size: 6.7 MB (6742957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3130d9160c32e3b47498ceb2ea232bdfdcd2fe0f470cb2df5f4a0e0ff919f9f`  
		Last Modified: Thu, 27 Jan 2022 05:49:33 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:fa0f8012a8ceeac28c9807c4cbc45134c9f690968a23742ceca3c631cb971c00
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
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
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
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
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
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
$ docker pull nats-streaming@sha256:4b10903c08537a97e6b945cdaaa0163fd5f83287e4807da303b06a6bb916c0ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:8208976899bae2b07c52ed71ba15d3006a8ea342e751fe2071d134c7d97702c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7039723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feacf64f84db353574b80d0552104f93839360bb95e872e22139e42053e95742`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 23:29:13 GMT
COPY file:7cb6d7b391f88ad91a3d8b81c68623a0f3c92c9e73939aa4823b990ac9676822 in /nats-streaming-server 
# Thu, 27 Jan 2022 23:29:14 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 23:29:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 23:29:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4edc1ec2dc80f100e623e2dd8e3424851cca1d9950d197169f07aa9d5148a308`  
		Last Modified: Thu, 27 Jan 2022 23:30:03 GMT  
		Size: 7.0 MB (7039723 bytes)  
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
$ docker pull nats-streaming@sha256:a0f7ed70d4736b01f938cd162f44e535c77fbb81354796c8affd4f9718982430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6549164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a5de2a796589fc94a859279f330b86055a5cedbf0178be55100c4f1c564bc7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 28 Jan 2022 10:47:40 GMT
COPY file:53ebe1d974c3fb2c62fe1809246c7150e6c2f8463f160e956ece6b743f95b8b3 in /nats-streaming-server 
# Fri, 28 Jan 2022 10:47:41 GMT
EXPOSE 4222 8222
# Fri, 28 Jan 2022 10:47:41 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 28 Jan 2022 10:47:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2b3e83c8b0486c1fa2aca390eefded15c4bcfbe7898abe0c3df822cb894f57df`  
		Last Modified: Fri, 28 Jan 2022 10:49:39 GMT  
		Size: 6.5 MB (6549164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:914869f94268b390a923b18f68d361a52db8122753a2557936baf1ee26e7b164
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6470229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a309e28d4efdde4dee3074f6a51aff746b87b4c06a4bbed71988185c85e59ab`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 27 Jan 2022 05:48:55 GMT
COPY file:8720a79121901c2f53c331a49132991f11ec3f28fb10f5b6a41d7097cecd1939 in /nats-streaming-server 
# Thu, 27 Jan 2022 05:48:55 GMT
EXPOSE 4222 8222
# Thu, 27 Jan 2022 05:48:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 27 Jan 2022 05:48:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:10d48e610369adb731205f3e174258c831f690cbe438b07fdb77887e7fcb36c9`  
		Last Modified: Thu, 27 Jan 2022 05:49:57 GMT  
		Size: 6.5 MB (6470229 bytes)  
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
