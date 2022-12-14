<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats-streaming`

-	[`nats-streaming:0.25`](#nats-streaming025)
-	[`nats-streaming:0.25-alpine`](#nats-streaming025-alpine)
-	[`nats-streaming:0.25-alpine3.16`](#nats-streaming025-alpine316)
-	[`nats-streaming:0.25-linux`](#nats-streaming025-linux)
-	[`nats-streaming:0.25-nanoserver`](#nats-streaming025-nanoserver)
-	[`nats-streaming:0.25-nanoserver-1809`](#nats-streaming025-nanoserver-1809)
-	[`nats-streaming:0.25-scratch`](#nats-streaming025-scratch)
-	[`nats-streaming:0.25-windowsservercore`](#nats-streaming025-windowsservercore)
-	[`nats-streaming:0.25-windowsservercore-1809`](#nats-streaming025-windowsservercore-1809)
-	[`nats-streaming:0.25.2`](#nats-streaming0252)
-	[`nats-streaming:0.25.2-alpine`](#nats-streaming0252-alpine)
-	[`nats-streaming:0.25.2-alpine3.16`](#nats-streaming0252-alpine316)
-	[`nats-streaming:0.25.2-linux`](#nats-streaming0252-linux)
-	[`nats-streaming:0.25.2-nanoserver`](#nats-streaming0252-nanoserver)
-	[`nats-streaming:0.25.2-nanoserver-1809`](#nats-streaming0252-nanoserver-1809)
-	[`nats-streaming:0.25.2-scratch`](#nats-streaming0252-scratch)
-	[`nats-streaming:0.25.2-windowsservercore`](#nats-streaming0252-windowsservercore)
-	[`nats-streaming:0.25.2-windowsservercore-1809`](#nats-streaming0252-windowsservercore-1809)
-	[`nats-streaming:alpine`](#nats-streamingalpine)
-	[`nats-streaming:alpine3.16`](#nats-streamingalpine316)
-	[`nats-streaming:latest`](#nats-streaminglatest)
-	[`nats-streaming:linux`](#nats-streaminglinux)
-	[`nats-streaming:nanoserver`](#nats-streamingnanoserver)
-	[`nats-streaming:nanoserver-1809`](#nats-streamingnanoserver-1809)
-	[`nats-streaming:scratch`](#nats-streamingscratch)
-	[`nats-streaming:windowsservercore`](#nats-streamingwindowsservercore)
-	[`nats-streaming:windowsservercore-1809`](#nats-streamingwindowsservercore-1809)

## `nats-streaming:0.25`

```console
$ docker pull nats-streaming@sha256:7b4c55332edea87655db394c79d14d136adfed19ea0682c4bc251303567dba6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine3.16`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-linux`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-scratch`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2`

```console
$ docker pull nats-streaming@sha256:7b4c55332edea87655db394c79d14d136adfed19ea0682c4bc251303567dba6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25.2` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-alpine`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-alpine3.16`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-linux`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-nanoserver`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25.2-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25.2-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-scratch`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-windowsservercore`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25.2-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:0.25.2-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.16`

```console
$ docker pull nats-streaming@sha256:e81914ab4fe7447eaa19609b3d97ef06705e727c3781f93123cc46682dff5278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:817810dde65bec1eddf00bb911b5b98c5cd4bf022348d3e0f89f161c46840da7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10727161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2559fccd4f8c32253c08492a5fe5845131c30326428dc5e5fce026196e9082f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:35:13 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:35:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:35:17 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:35:17 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:35:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:35:17 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf7a1f53c2673094ef2477f3b0962290b95401bc815aa48e9168d95dcb4b25`  
		Last Modified: Sat, 12 Nov 2022 08:35:46 GMT  
		Size: 7.9 MB (7920469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d99aeab13b93df1ce70cbbefbd4432ca2dd64687d78a9503cbbd3ffbbaffea5`  
		Last Modified: Sat, 12 Nov 2022 08:35:44 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:9a84378f6b3a668fedf7d1908766712692a0427b503266badbfab6df61a983a4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10199935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdb717a997ff33a2c27c4e733da6080a7f1e6a30a5b470972fd6b5c6de78af9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:31:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 08:31:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 08:31:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 08:31:04 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 08:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:31:05 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a7266d1a66f2ea5b801d7764a52c8ee1d5693f9a6476b22dc66f3d99b171a7`  
		Last Modified: Sat, 12 Nov 2022 08:32:07 GMT  
		Size: 7.6 MB (7584409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1628b93aaed041cd2ed4718e5e62302bf5ab47b44d537da490b4fa040ee70e1b`  
		Last Modified: Sat, 12 Nov 2022 08:32:06 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:b2b3ec423704edec471faf6d4c57d892812027757fb8c4aa97255537a70004fd
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9995817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc32f0df9620c827713e111965cf77d4bd6eff53fe4a56562d4534d8351f552a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 16:04:11 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 16:04:13 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 16:04:14 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 16:04:14 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 16:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 16:04:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:180214698f74077e0eb6b8658703ee6ae21d61b258f469176c194359241e8b41`  
		Last Modified: Sat, 12 Nov 2022 16:05:19 GMT  
		Size: 7.6 MB (7576609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4021d0b15354056e35afae8cd207d047215bb1ea39c0ca58f51e1d19240b2420`  
		Last Modified: Sat, 12 Nov 2022 16:05:17 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:ca778943e5f90ed98acff12f9648ae2c3a21578623afef9bfebf2a79b49f8404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dc0a84c9f36fd674923539f491f501c0d857b0223c3c3c56cac515342227db3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:35:47 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Sat, 12 Nov 2022 04:35:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Sat, 12 Nov 2022 04:35:50 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Sat, 12 Nov 2022 04:35:50 GMT
EXPOSE 4222 8222
# Sat, 12 Nov 2022 04:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:35:51 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63798248065feda710b4713523655c77febcbb996582363fe8c7f3409f4ff5f6`  
		Last Modified: Sat, 12 Nov 2022 04:36:20 GMT  
		Size: 7.3 MB (7277445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e07236f67dbbb6a2886398ef3bcbccf3a5872498eec2846d9e1daea137bc54f`  
		Last Modified: Sat, 12 Nov 2022 04:36:18 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:7b4c55332edea87655db394c79d14d136adfed19ea0682c4bc251303567dba6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ab9236d137e3eebdb5117eca1e9d49e4d8f1a56d38b2db676b5be5c13ef89118
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:3116f75802b15cbfbfb68adb1318f57abdb69648520ce249d40ff53fa319ae63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114438001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee7bd47856e33003f070b70e768ae086edd9b760c07f97e385de0f14a91183b3`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:47:08 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:47:09 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf05c94533b9e1051ea0a4d36dc4bb2a67a0c650df7779716b9cb8ed3493f66`  
		Last Modified: Wed, 14 Dec 2022 02:47:52 GMT  
		Size: 7.8 MB (7762314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ef7d369250b3e193928c56335454a4718c8a27de0d57edc3dee918faae8fd`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a53b13239d4767d0ddacfec5024dffdb1bd1e10241471e839ee0de616c83e3b`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed0891e29dba3b1e5f8771b4e02d7aec15e0e52a51f5f51bc0a7cae3bbd99c3`  
		Last Modified: Wed, 14 Dec 2022 02:47:50 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:4ddb50b6f43dfb76ba44400dac36a4998155db22c3fa4b7ae513a65e6afda1ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:287d05564c4c6750f56fdda41f05e552d88ddf386a6e44e1cc834e0a65c0eb49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7637811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455b7760d72d079088195f9cc0441f3fe22e1b46ecc2b8f49b3cda5ec483adf`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:20:21 GMT
COPY file:89087473017a2e985e9741a8aa3ec73c208da928bb57f2f24e30c00a31eafa8a in /nats-streaming-server 
# Tue, 11 Oct 2022 23:20:21 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:21 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:20:21 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:66e24392f842ad35144e78bc3adad500757ab527859ee38957e527487ef8b47a`  
		Last Modified: Tue, 11 Oct 2022 23:21:01 GMT  
		Size: 7.6 MB (7637811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:7a9e727242f052ad7f1aef67b29982a8d3f8bd6ea7e8cc8c76f3c7d2b044c667
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fad641972f0ff8f1dab2e34dca1f8e4011c5d32c7607c5bff6949a6a86d90b`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 11:34:26 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Fri, 11 Nov 2022 11:34:26 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 11:34:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 11:34:26 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ac505d089b210f05398eb249b7f3065fef3921be727978b70df4c11955da8d8`  
		Last Modified: Tue, 11 Oct 2022 23:50:41 GMT  
		Size: 7.3 MB (7300810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:45afd9c11672161333d5775564d46f19d15ba48f4a1bbd188da2e79c5d7b4a07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7288898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a8f3428876076d61520fde190b5fc4f479e3f80a5d6c914c210470635215bd6`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 21:12:17 GMT
COPY file:bf11e23254626a7629546dd0e7e134984e019132c260d1733b972d9775ff8160 in /nats-streaming-server 
# Thu, 10 Nov 2022 21:12:18 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 10 Nov 2022 21:12:18 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:2d5acf820909de2ff213199833cde1d52214f332d026d6f0b3807d819e2f657d`  
		Last Modified: Wed, 12 Oct 2022 01:12:22 GMT  
		Size: 7.3 MB (7288898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bdfae072b67d1ab734914a443796e974f5a7d73caa19aa5ba1a7abb335155705
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e5a4af7852aeaf241bd9103b8dcf4f7a1e9bd382a49dcfadf25aa83a1c404a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 11 Nov 2022 08:57:36 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Fri, 11 Nov 2022 08:57:36 GMT
EXPOSE 4222 8222
# Fri, 11 Nov 2022 08:57:36 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 11 Nov 2022 08:57:36 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:2d940524c5ddb53843d3ea11e7cfdf334ba00de760e8798453142f79484ec689
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats-streaming@sha256:32e7e068751b13cbc4e31cc3da4aefbb44cb43ee527d5fd231352cfe5409d7ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2789139702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca1ebc22ef56a07825b42eb24436965ca53f0c7f1d90a5927de5e1945343716`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Dec 2022 02:43:22 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 14 Dec 2022 02:43:23 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 14 Dec 2022 02:43:24 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 14 Dec 2022 02:44:44 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Dec 2022 02:46:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 14 Dec 2022 02:46:58 GMT
EXPOSE 4222 8222
# Wed, 14 Dec 2022 02:46:59 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 14 Dec 2022 02:47:00 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45763e1b21a0e9704075a43fdf236f77aea4b232d0cf0706074dbd445efc2c2e`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7b2cf1bed66ae6c1148d4358551103cefe8a90833e39cfea9b68b8597e9258`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3753292136fc6baef90e12385ac171fe0925688fd6627767dc83ff29f7849`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de18cd6aa4518b9e9c883f74abe95a5b8b93c84e8968df13928fe8c1abc574f`  
		Last Modified: Wed, 14 Dec 2022 02:47:36 GMT  
		Size: 341.9 KB (341883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fe31f2af1588f8248d617bd8176e70b821e4d8b9fde6085a31fe3da0ed501b`  
		Last Modified: Wed, 14 Dec 2022 02:47:38 GMT  
		Size: 8.1 MB (8089331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1ebc3201728285148652bf7eb51cf20c367a60a616beb5a39feb5a168afe62`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249b64e683538c1df73bf9d6823ebe375df0762fa349e39b21d309792044819`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b481e3290e6eaefd32e1265fb3508d5cabe14f01e1c066dffbefde8e46f8d2`  
		Last Modified: Wed, 14 Dec 2022 02:47:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
