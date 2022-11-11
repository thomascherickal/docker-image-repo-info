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
$ docker pull nats-streaming@sha256:12b51d25dbeb4868a2e56a569ed845cc4683ff24ac7db83f0a7b899c1f70fd46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-alpine3.16`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25-alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-linux`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-scratch`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2`

```console
$ docker pull nats-streaming@sha256:12b51d25dbeb4868a2e56a569ed845cc4683ff24ac7db83f0a7b899c1f70fd46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-alpine`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-alpine3.16`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:0.25.2-alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:0.25.2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-linux`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-nanoserver`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25.2-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25.2-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-scratch`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-windowsservercore`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25.2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:0.25.2-windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:0.25.2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:alpine3.16`

```console
$ docker pull nats-streaming@sha256:9a9de95c5dbab93fe0291602cf53195b759c78f53cbc0ce52169dcc4c87aa083
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:alpine3.16` - linux; amd64

```console
$ docker pull nats-streaming@sha256:994809a2a1c9823c5498a571c38d3bf773ebc702b10749983dce45b7a42cf712
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10726919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a408e43ce29cd045b46218f708c6a8c44050248220f5db8e8f837b94e82972`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:20:12 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:20:15 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:20:15 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:20:15 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1169afb18c1b6bb90747fac0f8a05090272062e2e2d120fb1dacfe825d8838a`  
		Last Modified: Tue, 11 Oct 2022 23:20:42 GMT  
		Size: 7.9 MB (7920443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba67a538f93cdd3f5fd299df6156a9825e518c36aea1fb2ec60c068ba8b96a4`  
		Last Modified: Tue, 11 Oct 2022 23:20:41 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bd4e1721fe14a07230933c589ab5053fa11a7a41bd4e13ee214cfb77e3332052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10198839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2760abcfdaed550a4291f6a0f816ac313becd053fb6c52587cd2cc6eb8efe5cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:49:18 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:49:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:49:22 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:49:22 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:49:22 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c2c4a7761930fe72a4660e6dfe67e097164722ae9089469941f25ccde847d`  
		Last Modified: Tue, 11 Oct 2022 23:50:17 GMT  
		Size: 7.6 MB (7584453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4e3c81559103bf50f09ba1185198ffb427389ee5f2adfccd9036bd598a6f86`  
		Last Modified: Tue, 11 Oct 2022 23:50:15 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:faf3434ebc649e471e46178227ce0023767eac219b3c8159c97fa23147f213e9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9994068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fcdddbedc68bcef0c6f521202b0426a1c15867b547f56e6beb4a21956eeb2c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:12:01 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Thu, 10 Nov 2022 21:12:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Thu, 10 Nov 2022 21:12:04 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Thu, 10 Nov 2022 21:12:04 GMT
EXPOSE 4222 8222
# Thu, 10 Nov 2022 21:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:12:04 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c126325b2ef9cecf9483148aa2bd30a7c727bc8abf4e36d3910cec16b3dae4`  
		Last Modified: Thu, 10 Nov 2022 21:13:12 GMT  
		Size: 7.6 MB (7576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b05bb599644a9f314cab590a6ccf610fee9e11b60f25bedaa341e04c49771b9`  
		Last Modified: Thu, 10 Nov 2022 21:13:10 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:eefacef374baa2a9df54722a8302b6aa25232d92425ff9090dc9aa3503cc549c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9985338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9b4cebbbeeae9e3de2b0953e457e42f932dd0b1d4f306b3dcae8e06cf27af8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 11 Oct 2022 23:40:07 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Tue, 11 Oct 2022 23:40:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5b9d00190a19a1cc67ace91ce6ad0b3f80db60689f13d24e9918ab9257d9a57' ;; 		armhf) natsArch='arm6'; sha256='46b7d196fd7fa48499c4ab273349ff1ce69d67b973904f2e9c5dd4cc39ef7796' ;; 		armv7) natsArch='arm7'; sha256='b0f33c99e8e8a8c7f715cdc7ab8c307711f52debf9895e0bbd33f68cbec05fb5' ;; 		x86_64) natsArch='amd64'; sha256='55789d3b4c4b5d6ddf0045a42e48f2d1fd2d220a2f4b13f561576bbd00d57154' ;; 		x86) natsArch='386'; sha256='f3ed9e878748154faeea488110a5332678a956a4959da958d30232503ffeec88' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-streaming-server.tar.gz "https://github.com/nats-io/nats-streaming-server/releases/download/v${NATS_STREAMING_SERVER}/nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-streaming-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-streaming-server.tar.gz; 	rm nats-streaming-server.tar.gz; 	mv "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}/nats-streaming-server" /usr/local/bin; 	rm -rf "nats-streaming-server-v${NATS_STREAMING_SERVER}-linux-${natsArch}"
# Tue, 11 Oct 2022 23:40:12 GMT
COPY file:528000310df8681fb95f43d3bcf7c8086cd514c78673b1aadb984b1db3331559 in /usr/local/bin 
# Tue, 11 Oct 2022 23:40:12 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Oct 2022 23:40:14 GMT
CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c51fbe1deebb00e09f3dad1bf5ee1a48df411fa1145ab407ccf4b09967769b2`  
		Last Modified: Tue, 11 Oct 2022 23:41:01 GMT  
		Size: 7.3 MB (7277255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba2b08678f1033e4ef779c9174a7e0c43610967506b0b7c5bd17c590f2be592`  
		Last Modified: Tue, 11 Oct 2022 23:41:00 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:12b51d25dbeb4868a2e56a569ed845cc4683ff24ac7db83f0a7b899c1f70fd46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:b33b9d9cf97a3d87b8b1247410c6fa1c444f8b5713ac91bfc1c4c812186ee7ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:1f1e6264687708ba147bbd17d4d8c0dbe98259726ffc9bb6ea485fa585064a96
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114490570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e9db05f817ddff2380c6c06c5f0710aafb45b503d2b38a4e3c8cf28e6ea5268`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:20:03 GMT
RUN cmd /S /C #(nop) COPY file:8231e132ceae2f5beb184edb8fd6927d5df2cb8a2774f0cb9b809b1a9176fa02 in C:\nats-streaming-server.exe 
# Wed, 09 Nov 2022 18:20:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:20:05 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99f48e4ed4473a894a45d73f972fe18df0a98679b3c4301c3ef4c106a4c90fc`  
		Last Modified: Wed, 09 Nov 2022 18:20:52 GMT  
		Size: 7.8 MB (7762375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df1a9be4b1efdbcb89bb3b190b84cfbec9ab0eea4729cc2b7e3750a8e24df18`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08e4620648f95dc56478f2e325a786fd136adf51e18bd16695a4ae85df6a2c`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1ba207c958d270c4c71a6ccc34821c6bf32eb74a6239578be3ef5209c824`  
		Last Modified: Wed, 09 Nov 2022 18:20:50 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:a17231ccb3a621621e67f58875e4259228dc85f06664af13592a1a55b69f9c17
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
$ docker pull nats-streaming@sha256:a0ea64e674bfa549c3f1b49963b966e9c98d06286bec39c07453cbabc66c6c71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7300810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:473c598470df786ebad8a1f903d231dec4cfcfd37e97c7f9b47a2e7131d94b34`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:49:32 GMT
COPY file:f7568230fc06888b50a5f3da0004bb7dc7a70b1defec143315a57570b4b91602 in /nats-streaming-server 
# Tue, 11 Oct 2022 23:49:32 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:49:32 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:49:33 GMT
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
$ docker pull nats-streaming@sha256:622d183659dc2b52c4d995d78139ce5df56f79a95edb23accef6826b13207a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6994195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbb6421bb9138c633b44f1839404fc16066c1b89dd3d79e2f44d6575e8afd7c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 11 Oct 2022 23:40:23 GMT
COPY file:215fac5233cbc7ee50e4033b703c84c22a4b219b4ab4c43d7317bc92b89f206c in /nats-streaming-server 
# Tue, 11 Oct 2022 23:40:23 GMT
EXPOSE 4222 8222
# Tue, 11 Oct 2022 23:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 11 Oct 2022 23:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:921e27ff4fbea0ffa1980a0bb3e13d378b150d7a7167d0dae7a3efbdc4408e37`  
		Last Modified: Tue, 11 Oct 2022 23:41:25 GMT  
		Size: 7.0 MB (6994195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats-streaming:windowsservercore-1809`

```console
$ docker pull nats-streaming@sha256:fc9f3a4493f401deed6acdcadaff40c596751f6fc9b5cd6fd3a5597e876c4841
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats-streaming:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats-streaming@sha256:e432cca2b1fb2af40ca299e80a02579387266d13a256bf7a23dfd7125a0ae4a1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2787076749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13f247cbd55632a872bae42021882364e6678b369692b701f6ebb8e9b0ddc4d`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 18:16:17 GMT
ENV NATS_STREAMING_SERVER=0.25.2
# Wed, 09 Nov 2022 18:16:18 GMT
ENV NATS_STREAMING_SERVER_DOWNLOAD=https://github.com/nats-io/nats-streaming-server/releases/download/v0.25.2/nats-streaming-server-v0.25.2-windows-amd64.zip
# Wed, 09 Nov 2022 18:16:19 GMT
ENV NATS_STREAMING_SERVER_SHASUM=554b083bb17f8f2e9a875b888dbe74454648f86c6e02bc489d88713431025d9d
# Wed, 09 Nov 2022 18:17:30 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 18:19:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_STREAMING_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_STREAMING_SERVER_DOWNLOAD -OutFile nats-streaming.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_STREAMING_SERVER_SHASUM); 	if ((Get-FileHash nats-streaming.zip -Algorithm sha256).Hash -ne $env:NATS_STREAMING_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats-streaming.zip'; 	Expand-Archive -Path 'nats-streaming.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-streaming-server-v*/nats-streaming-server.exe -Destination C:\\nats-streaming-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats-streaming.zip; 	Remove-Item -Recurse -Force nats-streaming-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 18:19:40 GMT
EXPOSE 4222 8222
# Wed, 09 Nov 2022 18:19:41 GMT
ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 09 Nov 2022 18:19:42 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe863d992e0c58c9cf1632767e37ade6556903b1bb890c2a4dc02dffeaed78ef`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71a5994065b88d8a198293e12ac4530e9342de0f4d53860ee2743bd2d569013`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8e674abd79efbd197e128d166729af96bcf66ffb1646f10fb80dde56503f83`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec5f49fc868f6f3b72e2f76461f16e59f80e92a4186383b3baf71c06d3d2b21`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 359.2 KB (359194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0897e7aebc234f59c04916a3b53b2a9b5ac2bda1415cddcb71ddf1966d20bdfc`  
		Last Modified: Wed, 09 Nov 2022 18:20:35 GMT  
		Size: 8.1 MB (8119591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea295c4d678432a3afecc78785a990244c290159cc0851aa868efc70979b97`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938d3ad7b90133750f1d10713db202d85b54f492cb2aef146e304f77b66f49`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b500e39240181724cbcb1a40781d36fae94a34eef9f926a5c612644211b67f`  
		Last Modified: Wed, 09 Nov 2022 18:20:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
