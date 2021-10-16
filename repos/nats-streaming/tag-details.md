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
$ docker pull nats-streaming@sha256:6a0b243e9f33d303bed37be0e5b466ace7a506c503548e242a8bade77828d9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

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

### `nats-streaming:0.23` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-alpine`

```console
$ docker pull nats-streaming@sha256:b2daa902af6ddf2da6cb377558d4a36752006aed509bb56fef948bf939d93ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:b2daa902af6ddf2da6cb377558d4a36752006aed509bb56fef948bf939d93ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:3f83f9642ddffccf052e403b7a84d70f73cb55d995d7d63b7eee555208abc4f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-scratch`

```console
$ docker pull nats-streaming@sha256:3f83f9642ddffccf052e403b7a84d70f73cb55d995d7d63b7eee555208abc4f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:873f62867ca3ce6469cc8df73a8033cc5950c9fd9d1f9ff698e2837eb114202f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e026444822e3bdfcc8fa34afb681175afdd82054acaf29d923bbc383349741c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a83613ed75a649bbdc111fcc41762a123f509d62a640b60feda55d787e9ba294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0`

```console
$ docker pull nats-streaming@sha256:6a0b243e9f33d303bed37be0e5b466ace7a506c503548e242a8bade77828d9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

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

### `nats-streaming:0.23.0` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-alpine`

```console
$ docker pull nats-streaming@sha256:b2daa902af6ddf2da6cb377558d4a36752006aed509bb56fef948bf939d93ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:b2daa902af6ddf2da6cb377558d4a36752006aed509bb56fef948bf939d93ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:3f83f9642ddffccf052e403b7a84d70f73cb55d995d7d63b7eee555208abc4f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23.0-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23.0-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-scratch`

```console
$ docker pull nats-streaming@sha256:3f83f9642ddffccf052e403b7a84d70f73cb55d995d7d63b7eee555208abc4f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
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
$ docker pull nats-streaming@sha256:873f62867ca3ce6469cc8df73a8033cc5950c9fd9d1f9ff698e2837eb114202f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:0.23.0-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.23.0-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e026444822e3bdfcc8fa34afb681175afdd82054acaf29d923bbc383349741c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:0.23.0-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.23.0-windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a83613ed75a649bbdc111fcc41762a123f509d62a640b60feda55d787e9ba294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:0.23.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:2a7a810a5bb19349a2e43fcb4f4cf22f83374b98aff961745b3d2b4cd6ebba92
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:2a7a810a5bb19349a2e43fcb4f4cf22f83374b98aff961745b3d2b4cd6ebba92
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
$ docker pull nats-streaming@sha256:709bf964baa04bed21788daab878aaf76613f67b25782dfa91f68dac883c1e96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9352403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120c9c54d0d41980417a67786d13b07474948f1a4fe697b1bfe029344e8b5d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:15:57 GMT
ENV NATS_STREAMING_SERVER=0.22.1
# Fri, 27 Aug 2021 21:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='581698d248a19ecae64e4048d153bc1021744a3da6284680a339f9f82a53a9cf' ;; 		armhf) natsArch='arm6'; sha256='438a89221bb0608e40d21e73ca27a4b70b8560730726942c0ade94a6b6013d6f' ;; 		armv7) natsArch='arm7'; sha256='4164baadd201d1374f7654d3e54a24d81ceb87a385867e31a82c1d1a69e3b1ae' ;; 		x86_64) natsArch='amd64'; sha256='f29e87ac9ff998c928aa8ebc8cf0c4d04d34a3d95b9900d92fd7dafab2bec8cc' ;; 		x86) natsArch='386'; sha256='0ca68e57babb8901d7afeb7569042730904887e718ddf860ef3ee54278753505' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:16:03 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Fri, 27 Aug 2021 21:16:04 GMT
EXPOSE 4222 8222
# Fri, 27 Aug 2021 21:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:16:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d0e8657e131875280f89b03741d9c7b5b154791cef8ce515fe711e4185a32d`  
		Last Modified: Fri, 27 Aug 2021 21:17:51 GMT  
		Size: 6.9 MB (6921563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506d2b8361ef74d3f9c4e5dc7489f829d0181c070aca1b163eb8f540762e4c`  
		Last Modified: Fri, 27 Aug 2021 21:17:47 GMT  
		Size: 421.0 B  
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
$ docker pull nats-streaming@sha256:ae45ed8e1202c415b0e0412ea3fd5128e668464815cb116b728e7b0517f36dc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

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
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
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

### `nats-streaming:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:16122e63a754b675121e8f119b76fa442df0a4ce9d559a7ca753d0f226e322a1
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
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
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
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:9f3f435b87851e7f36d57a5b75c245da6f89f4130d734145c8a108ab38fc69e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:a02439cb0d596ea38f885ba8b53e2540c94d7725d325c596261291e742cfd4ce
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110071703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e778f00d9162168523aea6a0fb2a246a46a183a5eddbbee466f0ebbbbac294`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:41 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Fri, 15 Oct 2021 23:17:42 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:43 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:44 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41032d84bba00f0810c799b3ced8dff4af2fc2493b0344d0d1f63ba81e5f3a19`  
		Last Modified: Fri, 15 Oct 2021 23:21:44 GMT  
		Size: 7.4 MB (7406064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6a7b297ef839c4d19eaa0f38f00d2741d476e6efcce70a66589818b00c7032`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12236ad1442efd152f0a101cd73c9a8d2930a207d741ea6afde8dfcd224e716f`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.0 KB (1049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e93ff25830548cd4d250e365bc463726a21f072157aecaa441af10213a75a`  
		Last Modified: Fri, 15 Oct 2021 23:21:42 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:16122e63a754b675121e8f119b76fa442df0a4ce9d559a7ca753d0f226e322a1
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
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
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
$ docker pull nats-streaming@sha256:873f62867ca3ce6469cc8df73a8033cc5950c9fd9d1f9ff698e2837eb114202f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:e026444822e3bdfcc8fa34afb681175afdd82054acaf29d923bbc383349741c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats-streaming@sha256:9dadfac2c2164b2db2f437d280a96d23909f72c4cf54645640144ffab451b1ee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2694437235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5263b600f73c9897a25a6ad86f6e57e29f9e8b17ce3469d56510db758c6bbf8c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 00:34:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:34:11 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:14:42 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:14:43 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:14:44 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:15:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:17:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:17:19 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:17:20 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:17:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55c74bf8af074a49872e1e0411ac5572625083d17cb1100c5cade611deeb92ff`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c196111fa2b96deb4010edf39b6c187a5308e45e859c0a062794c2fb5f3f48e`  
		Last Modified: Wed, 13 Oct 2021 00:43:40 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be5c409e035db76b6c76c2774e8b8209f20e1834a37862ad68a84c7518b0608`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141803b019a1fc302b56dcb3342baf0756b88480ca4d083ee358589caca2efc9`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dc43e6818218b07cf5b6a72f0a86a81a424c7578e183c8748bc7e03b2784f5`  
		Last Modified: Fri, 15 Oct 2021 23:21:31 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93af83f772b4d8e59adbfeb537345c8d87986cedc1b34413bd84d701cb7715aa`  
		Last Modified: Fri, 15 Oct 2021 23:21:29 GMT  
		Size: 358.7 KB (358738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4250c6ad05f6afb5a141b32358734851a7809aa0b8fe53ecea199340cee0505b`  
		Last Modified: Fri, 15 Oct 2021 23:21:30 GMT  
		Size: 7.7 MB (7749250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abe0499859e7991ff7935e2cd570691e4145343846b3f1916c20e63e83de1b`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aeb892ccb21479cd1d2461a9b2d91e8a660bfd99b6196f98cfbb187ca564ac8`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405241735b53c04f1deb99e0d57e4306a7000929fc1417f3b611e7941893ecd4`  
		Last Modified: Fri, 15 Oct 2021 23:21:28 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-ltsc2016`

```console
$ docker pull nats-streaming@sha256:a83613ed75a649bbdc111fcc41762a123f509d62a640b60feda55d787e9ba294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats-streaming:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats-streaming@sha256:8815df5da56bd4d4c6590ee3694d006ef79370de372711e6d9cc58883dc7eb58
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285418812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fcab03497c9b249c4819f3d431685eb7b5310f184c8173cc4a23fc43794bd6`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 00:39:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Oct 2021 00:39:25 GMT
ENV NATS_DOCKERIZED=1
# Fri, 15 Oct 2021 23:17:50 GMT
ENV NATS_STREAMING_SERVER=0.23.0
# Fri, 15 Oct 2021 23:17:51 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.23.0/nats-streaming-server-v0.23.0-windows-amd64.zip
# Fri, 15 Oct 2021 23:17:52 GMT
ENV NATS_STREAMING_SERVER_SHASUM=5b8196e5a8e3dd37de7e70df2787e2816d14da377c7ec0cf655df0a9fba3442f
# Fri, 15 Oct 2021 23:18:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 15 Oct 2021 23:20:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Fri, 15 Oct 2021 23:20:42 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:20:43 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Fri, 15 Oct 2021 23:20:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4d3c52a3fe41298469bd9ca8471cd22a349f75bf82b049e968c97dd7cbf538b9`  
		Last Modified: Wed, 13 Oct 2021 00:44:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5e5e67c70d509eb320faa6c55dd5fdc5c5440334d85dd07ea0e919299624b2`  
		Last Modified: Wed, 13 Oct 2021 00:44:15 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ed15de932d9979c2d43b9f3222f1bf63ac1e93c8957e8d111528f4eb10542a`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff05220fb197a9cf75d8415d18be45957137cfe4478eaf248f84d7c9d4bbfb8b`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9438d74b0196c77383038699d9a8499be3a062d6b3b9024e49979f93ec5d413`  
		Last Modified: Fri, 15 Oct 2021 23:21:57 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80833d1dbf80f7fb07f4604ae2e1ff98f6126193d8f1969528e6ac07d099dc5`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 348.4 KB (348369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b865d05ebabc15dffdec813d3c290e511d422ed598bbc88873c082770a3c451`  
		Last Modified: Fri, 15 Oct 2021 23:21:58 GMT  
		Size: 12.3 MB (12292917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a8815ed14c2b91e2a24342e413e5b71803558098b12872ea78541ed0342442`  
		Last Modified: Fri, 15 Oct 2021 23:21:55 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fe138b6fad8ac92c6b741ae450ccde60b6c4a6f8128dcb6e6459c19a0251bb`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e70c279d1c015efeca65bf0b0a05c18186bbb007b19fab36f0f87f311db5a4`  
		Last Modified: Fri, 15 Oct 2021 23:21:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
