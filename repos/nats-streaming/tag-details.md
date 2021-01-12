<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.20`](#nats-streaming020)
-	[`nats-streaming:0.20.0`](#nats-streaming0200)
-	[`nats-streaming:0.20.0-alpine`](#nats-streaming0200-alpine)
-	[`nats-streaming:0.20.0-alpine3.12`](#nats-streaming0200-alpine312)
-	[`nats-streaming:0.20.0-linux`](#nats-streaming0200-linux)
-	[`nats-streaming:0.20.0-nanoserver`](#nats-streaming0200-nanoserver)
-	[`nats-streaming:0.20.0-nanoserver-1809`](#nats-streaming0200-nanoserver-1809)
-	[`nats-streaming:0.20.0-scratch`](#nats-streaming0200-scratch)
-	[`nats-streaming:0.20.0-windowsservercore`](#nats-streaming0200-windowsservercore)
-	[`nats-streaming:0.20.0-windowsservercore-1809`](#nats-streaming0200-windowsservercore-1809)
-	[`nats-streaming:0.20.0-windowsservercore-ltsc2016`](#nats-streaming0200-windowsservercore-ltsc2016)
-	[`nats-streaming:0.20-alpine`](#nats-streaming020-alpine)
-	[`nats-streaming:0.20-alpine3.12`](#nats-streaming020-alpine312)
-	[`nats-streaming:0.20-linux`](#nats-streaming020-linux)
-	[`nats-streaming:0.20-nanoserver`](#nats-streaming020-nanoserver)
-	[`nats-streaming:0.20-nanoserver-1809`](#nats-streaming020-nanoserver-1809)
-	[`nats-streaming:0.20-scratch`](#nats-streaming020-scratch)
-	[`nats-streaming:0.20-windowsservercore`](#nats-streaming020-windowsservercore)
-	[`nats-streaming:0.20-windowsservercore-1809`](#nats-streaming020-windowsservercore-1809)
-	[`nats-streaming:0.20-windowsservercore-ltsc2016`](#nats-streaming020-windowsservercore-ltsc2016)
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

## `nats-streaming:0.20`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine`

```console
$ docker pull nats-streaming@sha256:478b026cdd046cad268dfc1d81fd3728e60b51bb0190c3412b0672a2d8903707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-alpine3.12`

```console
$ docker pull nats-streaming@sha256:478b026cdd046cad268dfc1d81fd3728e60b51bb0190c3412b0672a2d8903707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-linux`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20.0-scratch`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20.0-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20.0-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20-alpine`

```console
$ docker pull nats-streaming@sha256:478b026cdd046cad268dfc1d81fd3728e60b51bb0190c3412b0672a2d8903707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-alpine3.12`

```console
$ docker pull nats-streaming@sha256:478b026cdd046cad268dfc1d81fd3728e60b51bb0190c3412b0672a2d8903707
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-linux`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-nanoserver`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20-scratch`

```console
$ docker pull nats-streaming@sha256:e81347933b8b81d3c33c7de9b45bb84471a8f3e6c51ad098f1291e4e62a5ab0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats-streaming:0.20-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.20-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.20-windowsservercore`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:0.20-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:8a523efff216bc402aa3cfbff2baa00cba890204bd3640ee99cfd9af9b71dc1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f23e7901e6678f9427131aadcc75a95a91fb4c2ba46a005db8845ba1d5c7787f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67196f7de933f886026693bcb22ad853be6e6281c017c14733ad17f9339349c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:45:28 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 13:45:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 13:45:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 13:45:33 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 13:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:45:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a51653d4053c34377310b5008de57d6224fbbb3065b8d39c2623ec0d79976`  
		Last Modified: Thu, 17 Dec 2020 13:46:30 GMT  
		Size: 6.8 MB (6770293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e070c7a0e34ad8644a164b7ddd81ba5780220bbf304ff6280e5386c323eb2ac0`  
		Last Modified: Thu, 17 Dec 2020 13:46:28 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:327bffde98442421664114980572e9829a9b3d94d3d0ddd6f0454298c3b07035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8732352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6711b5f18d82236af21f862d8fcd2c2bfdcd38d5309184bd617c20b305ddd5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:47:40 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 01:47:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 01:47:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 01:47:47 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 01:47:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4690136a7acc690baaa780fd5921752acda2b6fe1e6ec277bc354a6d4162b8ea`  
		Last Modified: Thu, 17 Dec 2020 01:48:23 GMT  
		Size: 6.3 MB (6324375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9de5ac561e04e3c2bd7c49b1cdcc1cb937c6f42db6a00b057f6b94617ae760b`  
		Last Modified: Thu, 17 Dec 2020 01:48:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.12`

```console
$ docker pull nats-streaming@sha256:8a523efff216bc402aa3cfbff2baa00cba890204bd3640ee99cfd9af9b71dc1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.12` - linux; amd64

```console
$ docker pull nats-streaming@sha256:f23e7901e6678f9427131aadcc75a95a91fb4c2ba46a005db8845ba1d5c7787f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9569779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67196f7de933f886026693bcb22ad853be6e6281c017c14733ad17f9339349c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:45:28 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 13:45:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 13:45:33 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 13:45:33 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 13:45:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:45:34 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a51653d4053c34377310b5008de57d6224fbbb3065b8d39c2623ec0d79976`  
		Last Modified: Thu, 17 Dec 2020 13:46:30 GMT  
		Size: 6.8 MB (6770293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e070c7a0e34ad8644a164b7ddd81ba5780220bbf304ff6280e5386c323eb2ac0`  
		Last Modified: Thu, 17 Dec 2020 13:46:28 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:18fd3ddc15d5b65b6ad1171abf76e359cca31b60730750546e0dc0368a805750
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0322ce6374b271fc98c0e0a12b42c00a722465006d75394c2ab41bbb47d50c46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:53:38 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:53:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:53:43 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:53:44 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:53:45 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54831e858eddfe2c245e8c154d4422ad61bc9a30c1cfe612ec35f7a12b1e529`  
		Last Modified: Mon, 11 Jan 2021 23:54:22 GMT  
		Size: 5.7 MB (5726171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a9e8bb4d16b7ddec81004c2205411fc7b8830d0d2a0f3054a2fe0dc4664cd`  
		Last Modified: Mon, 11 Jan 2021 23:54:20 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:327bffde98442421664114980572e9829a9b3d94d3d0ddd6f0454298c3b07035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8732352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6711b5f18d82236af21f862d8fcd2c2bfdcd38d5309184bd617c20b305ddd5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:47:40 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Thu, 17 Dec 2020 01:47:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='d582023b8f9fe33b98f0faa6396aae8d5366ecade7e56cde912e21e5b93ea670' ;; 		armhf) natsArch='arm6'; sha256='f4af03e6cbb19f3ad9ea57217607dcf4b68018e1879859c847e2680917fc7139' ;; 		armv7) natsArch='arm7'; sha256='ec8c5ca693344e8b24de9ac955c38de757af8c5760658fc29ed2fbd804803fad' ;; 		x86_64) natsArch='amd64'; sha256='fc15530faec66b61de5140c2b99927c5839caff1c4c17f8bffbf4432fab83017' ;; 		x86) natsArch='386'; sha256='655f0f7cebf727317974006ad4a13ddacd3520f15266e854c2b01681e499bf80' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 17 Dec 2020 01:47:46 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 17 Dec 2020 01:47:47 GMT
EXPOSE 4222 8222
# Thu, 17 Dec 2020 01:47:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:47:48 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4690136a7acc690baaa780fd5921752acda2b6fe1e6ec277bc354a6d4162b8ea`  
		Last Modified: Thu, 17 Dec 2020 01:48:23 GMT  
		Size: 6.3 MB (6324375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9de5ac561e04e3c2bd7c49b1cdcc1cb937c6f42db6a00b057f6b94617ae760b`  
		Last Modified: Thu, 17 Dec 2020 01:48:21 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ae8f52346c3d26a49ae885bf56785f3952c14c8622a97e18288ae0abedd51660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8377876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f79e7574653a33192a8af07510cf1a7f03f5c02a77b49072304e701cf514cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Mon, 11 Jan 2021 23:47:10 GMT
ENV NATS_STREAMING_SERVER=0.20.0
# Mon, 11 Jan 2021 23:47:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='618008a4902916b6bdb26022343ab91313d4f7fc90b31d0c71ad9e75dc8299e4' ;; 		armhf) natsArch='arm6'; sha256='144b04f8f42793aee1b2deb3f6eb187648c37dcc32d526c607a0af99a847260d' ;; 		armv7) natsArch='arm7'; sha256='720f4a90d1dd536bc04639ae31c70ab46fb3e10556f0f261eb038fdce941f20c' ;; 		x86_64) natsArch='amd64'; sha256='098e2293cce5d457b92f3df35127789422562f1414427c406ffd03ea3bd687c9' ;; 		x86) natsArch='386'; sha256='322a290f4706f14d6ff8160ec437202bd282f61f0607741d0e4c38ef89b83451' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.zip "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-streaming-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-streaming-server.zip "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server"; 	rm nats-streaming-server.zip; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rmdir "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 11 Jan 2021 23:47:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Mon, 11 Jan 2021 23:47:15 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Jan 2021 23:47:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e424273d6cedd00225b67fa1b47e0dd8bf4b2abfa19fbc27f7763f096aeb138`  
		Last Modified: Mon, 11 Jan 2021 23:47:54 GMT  
		Size: 5.7 MB (5668408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33979e718e15555239006f224ba6d995cf9d6d044a7f25493196839d4d5aed73`  
		Last Modified: Mon, 11 Jan 2021 23:47:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:4950fb85fb1a07d1c97f57030f9ec7074b945077d5aeecd951a3377de9740cd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:916c386ed8189a8cd63b0c83e9a7f66447b0e3659c1c96fa6015589344c723b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a013f6e621b040ed030861cb0bd02d96ef23c7a5fbf2019841921e255379ebf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:9444afab14740d43bfd213340272edcfaa96f83b2ae24d586333398cc089a858
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107783475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bdcab4235f3b70b1671972c4154790bde79e33644ae254ae48efa965b2b3cb`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 17:38:01 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:19 GMT
RUN cmd /S /C #(nop) COPY file:cc6bae0f50b6e35b12e8233f240d95e093f7e44257bc87e06aed691866ec1477 in C:\nats-streaming-server.exe 
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:21 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:22 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8a3891744a5ba41f01e625a0a70d755ffe93de4d4f124ad6d069420d5c7956d4`  
		Last Modified: Wed, 09 Dec 2020 17:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2cf2a7f92a640dc1125e539b41a28abc6b4e2df892f67cbc0072f90bb65509`  
		Last Modified: Wed, 09 Dec 2020 23:08:42 GMT  
		Size: 6.5 MB (6515155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf561da2a706a067845b617e3efccdaf8257da5fb1ae53c383e29559f5220612`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e5e4a71ea08fded20e3471625c1c06c12540fd3c7f4e12eeaee288bf6e5377`  
		Last Modified: Wed, 09 Dec 2020 23:08:39 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7a7dbf47aa9dfd9ed44ec162d12b58d6751c6d5f129c4e65250e21fde3631`  
		Last Modified: Wed, 09 Dec 2020 23:08:41 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:916c386ed8189a8cd63b0c83e9a7f66447b0e3659c1c96fa6015589344c723b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:78cddd38d3c26f2a74454532132969b5fbc9fbff9cc8708cf338c1b33a80c17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:3a285fa7c8c148aad627e61b6848554ccc223cb30a1eb3293a5a5fb89af016c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull nats-streaming@sha256:7a8ab0956821d178ef84f6f10c399d44005ca86dd75378d41a5980979ed24409
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2411449594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0146757e90d9c2df66c7933b807c71d62de612813d33a32f15c8d7fdd710ddae`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:36:04 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:02:20 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:02:21 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:02:22 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:02:52 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:04:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:04:10 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:04:12 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:04:13 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b9257be76bd37cad15d45905ec5910266409794a9dbd8a0428174f8b2f352a`  
		Last Modified: Wed, 09 Dec 2020 17:42:00 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36644685392e418bf32ab96db81c8f6a861b913256c244637d9d3ee45098a9cb`  
		Last Modified: Wed, 09 Dec 2020 23:08:22 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9469bed00eb5f6a5b7c050a1aaee856134ec78bab6076cc793e26dc52ec71fa`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e9d451908e3e8ec10448e052cf25767a282312e49e29d2a0b42652cf217e28`  
		Last Modified: Wed, 09 Dec 2020 23:08:21 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870e3bb830bd8ad9b84a928d2b858be730dcdba8016206ee4aeda623d98754b3`  
		Last Modified: Wed, 09 Dec 2020 23:08:20 GMT  
		Size: 4.8 MB (4843348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d24c0a2fc2b3ecd1b0467794ae95667a29e1bd550bf2bf9c455499839253bc`  
		Last Modified: Wed, 09 Dec 2020 23:08:23 GMT  
		Size: 15.7 MB (15722612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09371bf015245c95ce8d5db6b8d7f90fc6d8527f83101535c8c6af719b628e79`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff8db511e98efbde9cbbf6ecd2d9bd2b73565c7c4e0d24dddeb6edfa2a1875`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13217bf3886546791bd6c26ab23636f9bc595fd80abf1e7d6ab6f10f8613cdee`  
		Last Modified: Wed, 09 Dec 2020 23:08:18 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:da877310cb87d1822f44a79a76b57af2eceb3e15aa82ab406a47d32bc0de9f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull nats-streaming@sha256:33a909f6239f294532f68e91f94655aa881f2c8701293c9963e4b1c85b1a1a52
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5790922042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e094a16d960a68e3691347bc7923c1f94b7db31dedb2ef74b9d87436170384`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 17:38:10 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Dec 2020 23:04:27 GMT
ENV NATS_STREAMING_SERVER=0.19.0
# Wed, 09 Dec 2020 23:04:28 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.19.0/nats-streaming-server-v0.19.0-windows-amd64.zip
# Wed, 09 Dec 2020 23:04:28 GMT
ENV GIT_DOWNLOAD_SHA256=edafd6482bd71f3d6035d7f6871df1fd4c53acf0ac19e88b85e08a2c7ab1cec5
# Wed, 09 Dec 2020 23:05:39 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Dec 2020 23:07:44 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Dec 2020 23:07:45 GMT
EXPOSE 4222 8222
# Wed, 09 Dec 2020 23:07:46 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Dec 2020 23:07:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d972336c8bcee0026c76e8f199cef405112a70aeef9917f07d2859f15162c1`  
		Last Modified: Wed, 09 Dec 2020 17:42:56 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4f52064be159ebf6d7d967a842e39ae04b53dcf15dd8b582a77af431f81df7`  
		Last Modified: Wed, 09 Dec 2020 23:09:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d1ecc24d286c8499d1698affa71481762f11bb3d4fdd9d35763dcbe94e9e9a`  
		Last Modified: Wed, 09 Dec 2020 23:09:00 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649366889ec5703d27a79142f0331f2a462858d6d6ee2a7c1bd8e426bece4236`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9916349c9d6afe29e7418ee0e8f0454bb37038070600eaef872fb7356c1147d0`  
		Last Modified: Wed, 09 Dec 2020 23:08:59 GMT  
		Size: 5.5 MB (5528923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838e032e6db488d413de3f4681555d2b57bb4472c3b16ed16a5c07f2e921f1ed`  
		Last Modified: Wed, 09 Dec 2020 23:09:01 GMT  
		Size: 16.5 MB (16540005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5c8ab334a9fbf340bbb2d213d16e91599eee98aafa72f7f8fbb6d4d147b27`  
		Last Modified: Wed, 09 Dec 2020 23:08:56 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db5c24070ad330bcb0f078a2325aba107a3a8615fc004248d02e8e828fa8ce`  
		Last Modified: Wed, 09 Dec 2020 23:08:58 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21108015f9c4f2ee78087806b4ca0582f2618489ed4899b07b6290d743b8ef3d`  
		Last Modified: Wed, 09 Dec 2020 23:08:57 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
