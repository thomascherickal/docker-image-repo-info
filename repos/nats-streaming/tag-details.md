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
-	[`nats-streaming:0.24.5`](#nats-streaming0245)
-	[`nats-streaming:0.24.5-alpine`](#nats-streaming0245-alpine)
-	[`nats-streaming:0.24.5-alpine3.15`](#nats-streaming0245-alpine315)
-	[`nats-streaming:0.24.5-linux`](#nats-streaming0245-linux)
-	[`nats-streaming:0.24.5-nanoserver`](#nats-streaming0245-nanoserver)
-	[`nats-streaming:0.24.5-nanoserver-1809`](#nats-streaming0245-nanoserver-1809)
-	[`nats-streaming:0.24.5-scratch`](#nats-streaming0245-scratch)
-	[`nats-streaming:0.24.5-windowsservercore`](#nats-streaming0245-windowsservercore)
-	[`nats-streaming:0.24.5-windowsservercore-1809`](#nats-streaming0245-windowsservercore-1809)
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
$ docker pull nats-streaming@sha256:013b9aefebbd9e8f7a93a7d4002d35e8dd9c01bf83884a7027750fd1e4da134b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine`

```console
$ docker pull nats-streaming@sha256:66ece185e763eac3ca83776148378735c40686c711c49b9762bf77e4ffd5ac2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-alpine3.15`

```console
$ docker pull nats-streaming@sha256:66ece185e763eac3ca83776148378735c40686c711c49b9762bf77e4ffd5ac2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-linux`

```console
$ docker pull nats-streaming@sha256:dd5242dd75c8a96846ca829900e6d23e183ee503a8e7c0999a585e400267f5a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-scratch`

```console
$ docker pull nats-streaming@sha256:dd5242dd75c8a96846ca829900e6d23e183ee503a8e7c0999a585e400267f5a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.24-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5`

```console
$ docker pull nats-streaming@sha256:c85b7c2e8006516b7fc780ba4c7732d4dca0015aa8b8981aac877c78ab843672
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.5` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-alpine`

```console
$ docker pull nats-streaming@sha256:ded953a4e8bcab98a96844fae3538474204470fed8cae4bee31a2f9fbab03c4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.24.5-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-alpine3.15`

```console
$ docker pull nats-streaming@sha256:ded953a4e8bcab98a96844fae3538474204470fed8cae4bee31a2f9fbab03c4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.24.5-alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-linux`

```console
$ docker pull nats-streaming@sha256:d2f3b6dbee89a4127697067d6f4db58e16380ce7bc3c1156c0f659c46285f674
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.24.5-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-nanoserver`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.5-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.5-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-scratch`

```console
$ docker pull nats-streaming@sha256:d2f3b6dbee89a4127697067d6f4db58e16380ce7bc3c1156c0f659c46285f674
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.24.5-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.24.5-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-windowsservercore`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.5-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.24.5-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:0.24.5-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:66ece185e763eac3ca83776148378735c40686c711c49b9762bf77e4ffd5ac2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.15`

```console
$ docker pull nats-streaming@sha256:66ece185e763eac3ca83776148378735c40686c711c49b9762bf77e4ffd5ac2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.15` - linux; amd64

```console
$ docker pull nats-streaming@sha256:d8b049047bee9dd4fbe1fce8eeef2e56b8e42c212f0be37b1b55e793be38f639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10250419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b951b244987f70d60dfaa391436ab4443bcb7e6dd32b92d8496dbd4c6bd376b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:20:12 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:20:15 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a3272c04524d6cc3b02ed7f88bf1f295640ed810e95f871cc0a382c5a3cca2`  
		Last Modified: Fri, 22 Apr 2022 16:21:23 GMT  
		Size: 7.4 MB (7435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c45ebdb1c5282541c42dfdd91a69f1180e91de2fa6b2d7cdeef4270d8e42c8e`  
		Last Modified: Fri, 22 Apr 2022 16:21:22 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:796d10c768ca6f6144746d705a476c0b0991d7191e68d8562a3a2222890b6205
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9564190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0e2bf39b23cc821a7bb084ddbdf639ae9acf6a388b2bd3bc12d66cc86f7833`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:53:19 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:53:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:53:24 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:53:24 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:53:25 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d499f7f928072461e8c764725192c79438de20ce38b2f693c82858de92ea0271`  
		Last Modified: Fri, 22 Apr 2022 16:55:08 GMT  
		Size: 6.9 MB (6941796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f308cb69bb32912861b75333647e2a7d084bd8b945323a3cb3a587b7d366e`  
		Last Modified: Fri, 22 Apr 2022 16:55:03 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:43fa0020bbe495315ac2f09debe4bf6b27dd74790d26ac3366750c3055e58a3c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4afe09639533164664c235319932921bedc9450ecd3de243641a70c7a583c5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 18:57:51 GMT
ENV NATS_STREAMING_SERVER=0.24.4
# Tue, 19 Apr 2022 18:57:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='abf61454846309f4350a209aa86d8def4ceefaa35b576fe027915f31eeaaebf6' ;; 		armhf) natsArch='arm6'; sha256='bc6efafbf051b8bbabe868240ffa9f88a5676727e3c6a5ffc13542ebd0d6585c' ;; 		armv7) natsArch='arm7'; sha256='7950f6ea4b5385454350c8979d6062aa710400a2d21a3a44d971e8535d944545' ;; 		x86_64) natsArch='amd64'; sha256='e7b1db559c02d123d0aabdf0d3a93803eb0778aa733a26ec9067c833bd5728b9' ;; 		x86) natsArch='386'; sha256='941a7be15b8f3d2ba18508baaced39884b1ed86214c2afb2c2bcfcfad3743903' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 19 Apr 2022 18:57:56 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 19 Apr 2022 18:57:56 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:57:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 18:57:57 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab0ba64de7ddcb969882eb8b609a89179c2d441a4bcc7317ae977fd7dda4e23`  
		Last Modified: Tue, 19 Apr 2022 18:59:41 GMT  
		Size: 6.9 MB (6929861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e7fde7215edaedba408f2d6f77c7043df6c84d3309cffeb7f8b14f1c0b82c0`  
		Last Modified: Tue, 19 Apr 2022 18:59:37 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ffa711573fa73750390568245b90ee771dab9144f7a74cb7bf5efa6e2b1c4d02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1df12bc99f988acc78fccc9047027c17d839d4ddf40a9583586531f34aa83f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 22 Apr 2022 16:42:27 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:42:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='1cc0aa6328b4844aa22accaf8dbb0cb2624c7feae6b27a1a64f7da4dd86c1cda' ;; 		armhf) natsArch='arm6'; sha256='a691dc15fdb17d6d1d69f108d72c6a28d2151fa6abbddb2823c1624792b77c2c' ;; 		armv7) natsArch='arm7'; sha256='e93e783e2b89ca340fe623b5575375eb792de3b5ac180023f318faed8e648a58' ;; 		x86_64) natsArch='amd64'; sha256='d368b2cbc60fb37316ad139b978a5c830ba2400affd56910ecc9b363d16e0663' ;; 		x86) natsArch='386'; sha256='d553dc387e91573b8d3b7093039d9cc1392c95863bf20027c3ff4350a0cd9890' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Fri, 22 Apr 2022 16:42:31 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 22 Apr 2022 16:42:31 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Apr 2022 16:42:33 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd05bf869a3e992428717cb5c3f43ef5f65cb8f1fb9052ac0b538dedf80dbe`  
		Last Modified: Fri, 22 Apr 2022 16:43:24 GMT  
		Size: 6.9 MB (6852803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4679b108959e4509b6baaf39ffa3486224e9c1ce4243b0180cdfc954656f0983`  
		Last Modified: Fri, 22 Apr 2022 16:43:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:013b9aefebbd9e8f7a93a7d4002d35e8dd9c01bf83884a7027750fd1e4da134b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:dd5242dd75c8a96846ca829900e6d23e183ee503a8e7c0999a585e400267f5a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:e1cd08756767b3c71dd69e3a54e5c07795348788b1df3d08cc0e37df34774c85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:ff24a4fa3b2fdde5da8fb925db5485c904e17f9d8b9115d2eb9df879ab71fd83
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.4 MB (110374899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a421a5ba199461dcbce24329799099bed8d6c9317e3cb80601afad2cd0666e`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:18:55 GMT
RUN cmd /S /C #(nop) COPY file:e45fa44752e59260ce53c936e3ae69ead52147ef2900cdcfe6deddf6f13523df in C:\nats-streaming-server.exe 
# Fri, 22 Apr 2022 16:18:56 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:57 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:58 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c735b2414c606e5228ba5175f5459f1893a6b0926f2026a790ead05be0908`  
		Last Modified: Fri, 22 Apr 2022 16:19:47 GMT  
		Size: 7.3 MB (7274509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7c95272ff6285e639ba8cf376074f8359485b361091ebb1fdcc9685950774a`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4852fa43a27d4df369b87bd6843d238b3a9e3642f5c28235e6bc3b072d865f`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cde88fca97467c4c0820a06879f10b9192bb31b18dfbc0c5ff0dca1c88339d8`  
		Last Modified: Fri, 22 Apr 2022 16:19:39 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:dd5242dd75c8a96846ca829900e6d23e183ee503a8e7c0999a585e400267f5a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:fddd09ee25ee9c86b46c8757ecf745340df87dcc06eb95168406efb2132e40ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7163100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9386cfb5d02c44c24efbe824233636558940a5e147c986086a17d1fadb840`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:20:56 GMT
COPY file:0541fc2faebb84ec49eeb8436ad9f601e37d5d4790390e35c76a5edbe9103024 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:20:56 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:20:56 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:20:57 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:17e859136a3301ee3240f0c726d8e55e45359966535d9d3c8402c905d1a98cb7`  
		Last Modified: Fri, 22 Apr 2022 16:21:42 GMT  
		Size: 7.2 MB (7163100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:6b14356b4fd36c4830e22a7f91c2b6ad2ef4e400872e58893ac019b405a31263
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6668949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520d8b4d635a64a7821caf85c57ff9f9448f7a7c6e750bc3252dfd5a6ad009b8`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:53:44 GMT
COPY file:e967421ab3433299096179cb62ddc3e6b3f50f6a53eb2fdbdd4730f7062afd51 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:53:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:53:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:53:45 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3cd7674bffb9eff71229441c0f38770e6136618fa0bff85992f6e96039ff7227`  
		Last Modified: Fri, 22 Apr 2022 16:55:37 GMT  
		Size: 6.7 MB (6668949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:e8e52a390d9cefe82a9f17a19e2e05c49d4c56a27b05fb956108c047d5a93b31
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6657656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f1e8f63244361974ea334f20240f6d4f94fc96d7e89051e0769eece666b959`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 19 Apr 2022 18:58:20 GMT
COPY file:17bb63ff84cf537d44fe2a6c3b62b7c20b07b7ddd09ec3e118a9ee70593166c5 in /nats-streaming-server 
# Tue, 19 Apr 2022 18:58:20 GMT
EXPOSE 4222 8222
# Tue, 19 Apr 2022 18:58:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 19 Apr 2022 18:58:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:501cd5abe17e56e7e4b1c9fb82796e05c14f6dcbf6e964d8c37a33da0eb82757`  
		Last Modified: Tue, 19 Apr 2022 19:00:12 GMT  
		Size: 6.7 MB (6657656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bf346cbfc924bcf72a6531ac8a7d161c01fd25051260e30f9b0b745ae3253d46
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6579487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e87622b49967714ad1e0ead28ac1e58c75543cdb3359fd2677802cc714be946`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 22 Apr 2022 16:42:44 GMT
COPY file:dbd513a5600a60a94aa30be1078814e785fc59b70c15ac820d0ab1a582d4d0e3 in /nats-streaming-server 
# Fri, 22 Apr 2022 16:42:44 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:42:45 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 22 Apr 2022 16:42:46 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:37f1a36ce7b29667a50caf34413a6e43431d23052484a3f9510ee63ea49c1708`  
		Last Modified: Fri, 22 Apr 2022 16:43:47 GMT  
		Size: 6.6 MB (6579487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:1494fcfcf9e45883e52e94a5a589198fe8a805c98ac054a65637babe8d433281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats-streaming@sha256:b5c08f497b7034b40103afadb2de1ea80ffaec6f86d5df5ddb63c698218c15e6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2723900457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409a3a686843048ae4b1707085eafc137b83122eaa82cace3ed90569b7eced8`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 22 Apr 2022 16:15:54 GMT
ENV NATS_STREAMING_SERVER=0.24.5
# Fri, 22 Apr 2022 16:15:55 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.24.5/nats-streaming-server-v0.24.5-windows-amd64.zip
# Fri, 22 Apr 2022 16:15:56 GMT
ENV NATS_STREAMING_SERVER_SHASUM=8a4f4ff3a1262fc5fb348a0b58acc588d724daabc29c650d87183e3660faa074
# Fri, 22 Apr 2022 16:17:05 GMT
RUN Set-PSDebug -Trace 2
# Fri, 22 Apr 2022 16:18:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 22 Apr 2022 16:18:45 GMT
EXPOSE 4222 8222
# Fri, 22 Apr 2022 16:18:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 22 Apr 2022 16:18:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45166e7a394e3545f3f33cb3ddb87152f4fd62b71cd9fc15919d332960cd837`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15189228445a234e42f52b9d812173e26edba4d824b0aed5aeab7e820c227829`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957632d445179c10f7a677adbf9083301e0babafc9c02e4c960a0fcee0bc875a`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc01bf16f3fe2409e6d20d14a4331c53d33c60426c077e6fc1ccda46115184e`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 359.5 KB (359465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb1c69178bc5509d69253833c75bde1a0be47c2047c76d6a72c6d389da8ccbe`  
		Last Modified: Fri, 22 Apr 2022 16:19:27 GMT  
		Size: 7.6 MB (7610052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab4e62675e125fcc1e4d16af54f1f5d62fbff63745b0c24b6f03dfae2487bbc`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa2c4d46e180f44fa57fac356e03fb9b8a999c2b9ac826aeffff4bf91348852`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40aa7abe2b65926c6ddfd84dc6cc45248873effced7ad95a9c3a9aeeb3230f79`  
		Last Modified: Fri, 22 Apr 2022 16:19:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
