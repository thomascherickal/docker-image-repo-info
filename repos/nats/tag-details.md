<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.13`](#nats2-alpine313)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.2`](#nats22)
-	[`nats:2.2-alpine`](#nats22-alpine)
-	[`nats:2.2-alpine3.13`](#nats22-alpine313)
-	[`nats:2.2-linux`](#nats22-linux)
-	[`nats:2.2-nanoserver`](#nats22-nanoserver)
-	[`nats:2.2-nanoserver-1809`](#nats22-nanoserver-1809)
-	[`nats:2.2-scratch`](#nats22-scratch)
-	[`nats:2.2-windowsservercore`](#nats22-windowsservercore)
-	[`nats:2.2-windowsservercore-1809`](#nats22-windowsservercore-1809)
-	[`nats:2.2-windowsservercore-ltsc2016`](#nats22-windowsservercore-ltsc2016)
-	[`nats:2.2.6`](#nats226)
-	[`nats:2.2.6-alpine`](#nats226-alpine)
-	[`nats:2.2.6-alpine3.13`](#nats226-alpine313)
-	[`nats:2.2.6-linux`](#nats226-linux)
-	[`nats:2.2.6-nanoserver`](#nats226-nanoserver)
-	[`nats:2.2.6-nanoserver-1809`](#nats226-nanoserver-1809)
-	[`nats:2.2.6-scratch`](#nats226-scratch)
-	[`nats:2.2.6-windowsservercore`](#nats226-windowsservercore)
-	[`nats:2.2.6-windowsservercore-1809`](#nats226-windowsservercore-1809)
-	[`nats:2.2.6-windowsservercore-ltsc2016`](#nats226-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.13`](#natsalpine313)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)
-	[`nats:windowsservercore-ltsc2016`](#natswindowsservercore-ltsc2016)

## `nats:2`

```console
$ docker pull nats@sha256:a856b051aea8302cb1b376bc6066027e19b2a8275f6b0e9569988591f420e500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:15fd1b21e741820bc55474a7497badd960b5156ad837d1c04c7052500037eb8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:4247bc089c60804b09d260b2a2e1038ebce8d3d17794bdda9708ec00f9b7d801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c5fda78ae083ac9b43909766599a77289559545e8ddb747f2b7cb257a1dc184f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:a856b051aea8302cb1b376bc6066027e19b2a8275f6b0e9569988591f420e500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:15fd1b21e741820bc55474a7497badd960b5156ad837d1c04c7052500037eb8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:4247bc089c60804b09d260b2a2e1038ebce8d3d17794bdda9708ec00f9b7d801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c5fda78ae083ac9b43909766599a77289559545e8ddb747f2b7cb257a1dc184f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6`

```console
$ docker pull nats@sha256:242b56ba9ab44e5c16e5205fa6c1610244a7c7a607a76f52f821bc1797999130
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.6` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-alpine`

```console
$ docker pull nats@sha256:9b550d2edf33e9e828ffb5c3acfa8ce3565b352e821af5c20374ef28fa7cce29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `nats:2.2.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-alpine3.13`

```console
$ docker pull nats@sha256:9b550d2edf33e9e828ffb5c3acfa8ce3565b352e821af5c20374ef28fa7cce29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `nats:2.2.6-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-linux`

```console
$ docker pull nats@sha256:664898c45644c30a9984782c04a094a1a6d4c9fa1d0157aac01f04c76be93ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `nats:2.2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-nanoserver`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.6-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.6-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-scratch`

```console
$ docker pull nats@sha256:664898c45644c30a9984782c04a094a1a6d4c9fa1d0157aac01f04c76be93ab0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `nats:2.2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore`

```console
$ docker pull nats@sha256:15fd1b21e741820bc55474a7497badd960b5156ad837d1c04c7052500037eb8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.6-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.6-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:4247bc089c60804b09d260b2a2e1038ebce8d3d17794bdda9708ec00f9b7d801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.6-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c5fda78ae083ac9b43909766599a77289559545e8ddb747f2b7cb257a1dc184f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:7b65c778de18fe7a0e849098344166a05738caadb1d5a914cc4e8489b9b00a85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:9d2f79cec13b773e5677cec0f3272e52e55be44210e9f5b4917c623166394f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7345153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:491da5634208d92e0c0a052128e76069f3d086b42582b2a07515f1b2284e1b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 01:38:13 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:38:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 01:38:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 01:38:16 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 01:38:16 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 01:38:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cf50b10150a20d88392a1085f9599e8af8f5a3018685f039e7c0e5dd7288d4`  
		Last Modified: Tue, 25 May 2021 01:39:00 GMT  
		Size: 4.5 MB (4532213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ee7d5e3ce0eae646fccf205b9550e978ab7664d6926dbb673199ef0f8835fd`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a7f22a12d626460f4a81bc8142154fd148479c9c6d9c9513863790fc54ec43`  
		Last Modified: Tue, 25 May 2021 01:38:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:1c73109d6f0f4df4a01946b56cb9ee820e00ccab3a53a313fa455132eb429c5a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6817138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610510cf73d587ce2492ee376849f1ad1c1aa9c4302164b35201671f17e814f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:51:13 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:51:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:51:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:51:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:51:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:51:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:51:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3f71d1e179b53574a4255bcfcd71fe370c624cd262a2ab7aaffd8e5d31720a`  
		Last Modified: Thu, 13 May 2021 17:55:46 GMT  
		Size: 4.2 MB (4194035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e8d47bbf0baab0970aae54c06f1e44815789587f8278d70e26399b9c5b6a52`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36205a7a8707754144c7268ec085628e59b88815290a05666849b317dc5cf11b`  
		Last Modified: Thu, 13 May 2021 17:55:44 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:91d2dbf930b400b44b948361b60920659e74b28370d38b384bda56985d7d172c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6617719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02dc5ea95004c286602940e81b2950f498ef35217e01e1da4e372194c8a65d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Tue, 25 May 2021 22:22:45 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 22:22:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='779d7f363fb0244071e67bf146c7169a8e3c35af2746c0a01323a3c5fd12bf31' ;; 		armhf) natsArch='arm6'; sha256='ed7211f56fa3928e3664ed92df632b0e7480bd1b4a91c239cb26a0f55831c815' ;; 		armv7) natsArch='arm7'; sha256='a55335b1329248912e80d8e68b5dd6b6a48c4742de089c4226f503d7e8357f2c' ;; 		x86_64) natsArch='amd64'; sha256='fc67ce0b4c748fa16ff92414c7d6be18a9285824c21d9629684c0093cf074f77' ;; 		x86) natsArch='386'; sha256='386811034531cea6e794e4764fdd70b0b948fdf7212064e8c176663992c46f2e' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 25 May 2021 22:22:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 25 May 2021 22:22:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 25 May 2021 22:22:49 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 25 May 2021 22:22:49 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8fd93bac31720120ec97ee8f514ace788f281711084b9532b4d152e8fa3514`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 4.2 MB (4192604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240e54fb35db3d43766365af298a4fcd1eaab7acbfda0fd141a242fc1feaeb5`  
		Last Modified: Tue, 25 May 2021 22:24:21 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfddeffbc3b0f30d139487df21b514ec7bc915cbca61e31ee793eed0d9472e16`  
		Last Modified: Tue, 25 May 2021 22:24:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5d118edac8396ee73f73a2db080f4d870c52a48d1b7dfe932a8e3ec399e10ce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6878882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34f7d4fedb21f182edb7ca233e3ca03ce7ce1ffc9da57a002a1c6fc3d470b9ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:39:53 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:39:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:39:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:40:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0a5de4d48d58b6e52e98523137e1c70f8edaa9edaba04eef99d76177962a7f`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 4.2 MB (4165884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bc18d6dca6719f9820cf0786282a7083a2b6ba41f6004e3a6b4e9aef5db72`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f454ed6fd75994bba5f04bf38710b744a0804d5bec911593148cd24993d73d86`  
		Last Modified: Thu, 13 May 2021 18:51:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:a856b051aea8302cb1b376bc6066027e19b2a8275f6b0e9569988591f420e500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:067b5f74a2e8cca10de555e7c628051fdb2c25d8776e45c3ee524b887de18833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:ddfd365b806886e2c42b1dfd8987709f191bb672efcc19282ad97ede8b64ac6b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105687207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235754056e955f3cd979b7633a592ae74253e5b5fdbef62e31f0f1916792f0f1`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:29 GMT
RUN cmd /S /C #(nop) COPY file:a13acc0f2f64f12c4304c7730a47bebb73f06865d8dee680ec7a370c77d69e10 in C:\nats-server.exe 
# Tue, 25 May 2021 01:16:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:33 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f39f6a9f7f712e7e53aee1634305c4d79bac02566331c159233f7f1516f7ca`  
		Last Modified: Tue, 25 May 2021 01:21:47 GMT  
		Size: 4.3 MB (4305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a168ac318936785bd1573942ce0bdc26dd62bd9abf6d665bebf4eb5679fd5b`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31a654eec8e24806d907cd3e24518c46b33a321477dc6efabd572ca5be0d9be`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e5f1c9de2f651b9443457fe62ef1ddbf2b37d0d01f0474e564d63a2462a9a2`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b26efd0d2a66df6c625ae45d6f9011cfb543a9a09833d2360799085c89d17c`  
		Last Modified: Tue, 25 May 2021 01:21:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:754db44884ab2aea35d04ed50f539047af647866a31e7324f95f76a675518a7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:bad1b98cb238be899761405ed9a084eb4cee1e4982c4082414a49e1e47d83993
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4249359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3903d09e582715d83e8da5706ee14109824854452c0ebf177eb55dfb789e311`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 01:38:34 GMT
COPY file:6d5e77e6be5bafda9b9e03a4f397b21f9432694e3c3c3b5cd6e621b4c3ec3018 in /nats-server 
# Tue, 25 May 2021 01:38:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 01:38:34 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:38:34 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 01:38:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bf9e6d973acc267c8b0f05973d840142eec057566b36d0ae18177113f1fdadda`  
		Last Modified: Tue, 25 May 2021 01:39:26 GMT  
		Size: 4.2 MB (4248883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a60a1c8cdedd7b360929beb64e25bbab3d679ba8134844479aaa6169d73595`  
		Last Modified: Tue, 25 May 2021 01:39:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a983500bd3159616829a01eb09da7b6f158350af2fdcc128934412495425164
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307861f2de6658cd7862d3a7131fc2e28b87f2eb746894ea366012f2779d8fe5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 17:55:06 GMT
COPY file:d16ae4808e5ed65af2285b0f83247b43f50b4ea2032e34e3252016ed8c93c6f5 in /nats-server 
# Thu, 13 May 2021 17:55:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 17:55:08 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:55:08 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 17:55:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:118322ef642e61d559f02e2a4492d94d0d570f5bcba84e38cb7a6f3cf4edfbc2`  
		Last Modified: Thu, 13 May 2021 17:55:59 GMT  
		Size: 3.9 MB (3913497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3bce3e269b792229af46abac6142df986aa7890b4f095102ef1f638384339`  
		Last Modified: Thu, 13 May 2021 17:55:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:593e1b418f3e55050730f63b1d5da6e5f6f9c990c66e15bb9cd6659ea836279f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3914539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4093ac9e36206435159f30858c34c7ed656e69e8dcbe1aaa6fbd40099701ade7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 25 May 2021 22:23:02 GMT
COPY file:1ccce8553c778be1204380469e7248fd9ee472bdec35db0b7dd150122ae7c37d in /nats-server 
# Tue, 25 May 2021 22:23:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 25 May 2021 22:23:03 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 22:23:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 25 May 2021 22:23:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a459b50ce258c1a3884cfc6f671ebabe9d05421a39962966809134623f3b9979`  
		Last Modified: Tue, 25 May 2021 22:24:59 GMT  
		Size: 3.9 MB (3914063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1808b616cb182b07285cb2e4b7d289755ccf8fa8575a8bc73a20ae46f8f253a`  
		Last Modified: Tue, 25 May 2021 22:24:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:8e65e0b3431668fb0359dcb4fcaf23bb9191ce7ecb82e1a22a3be29ee36004e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3885342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:271e11288d98ed351e961eee8c1e7482b4aea58d23b2fa242145d9119f6b2196`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:50:57 GMT
COPY file:197c9f2a7ab883ce9e7b0cabc46d550567f9d5f5b9d7ad251fb1b3fd5f48c063 in /nats-server 
# Thu, 13 May 2021 18:50:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:51:00 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:51:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:51:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2e7bb276bfbe36686f13511ba31d8fd254b86cdcbe3471bee201597b3e35565`  
		Last Modified: Thu, 13 May 2021 19:51:55 GMT  
		Size: 3.9 MB (3884867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08aafee98345505bf1097023e5e040befb3e910fe2600472f61b4ac034c51763`  
		Last Modified: Thu, 13 May 2021 19:51:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:15fd1b21e741820bc55474a7497badd960b5156ad837d1c04c7052500037eb8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:4247bc089c60804b09d260b2a2e1038ebce8d3d17794bdda9708ec00f9b7d801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:a6f22067697199f80d68a74778c3bb9099a12d3dbc3278f7ef93be56d31fc183
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489016379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63fca474701f1f0e9d0281510b24cd932a253654182e1353b094e7a7463a9745`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:14:17 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:14:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:14:19 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:14:52 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:16:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:16:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:16:08 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:16:09 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:16:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5681a3e632e6d4bd2a711b5c2cca47977a6e5ed945d514b572c31df7f19745`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f567f9d954b6724b4214814bf6e803b5038783846e38cb5c3c00d1ac221e7485`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b114841fe84881638c234af552e84481883b24f5b5d55dd80c7f94adee103937`  
		Last Modified: Tue, 25 May 2021 01:21:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad08cab48fef4ae82821d23e672f68a60fe6c3b72e43cf4e5b04a22cba1b6c2`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 5.1 MB (5120734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b106ad516f3a3d8537118273dc114b81ab7c89605c00488b60ff048b523caa48`  
		Last Modified: Tue, 25 May 2021 01:21:28 GMT  
		Size: 9.4 MB (9393121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab0f8fce81fb7e4aa7999c009b7d42708f432535b434eeb7a3b7955972e9a1e`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d257ed611f6ef2b6ad85ac42d52b050147e41ce1458af9a512aad64e5d6e349`  
		Last Modified: Tue, 25 May 2021 01:21:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcac983a901b69680c4bf1be54a37e7699179731c32815f2a512eec2a95fc78`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34566e0d187b0ae056c41436f264780964d543281edfa2b90c0995351c5a98ae`  
		Last Modified: Tue, 25 May 2021 01:21:25 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:c5fda78ae083ac9b43909766599a77289559545e8ddb747f2b7cb257a1dc184f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:4449ca56d8bc1548ecfb8e5d401a0d816f0c57676120c55b9732b0d575a48dd8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815952656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1352581e4f64d1fe20d0794edda7888f9e58b046ad8c7a8617a2ae29d196eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Tue, 25 May 2021 01:16:42 GMT
ENV NATS_SERVER=2.2.6
# Tue, 25 May 2021 01:16:43 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.6/nats-server-v2.2.6-windows-amd64.zip
# Tue, 25 May 2021 01:16:45 GMT
ENV GIT_DOWNLOAD_SHA256=c1712f41e4e811027701a036b6ff67b1f09fb298b0674098b26f875d37e709b2
# Tue, 25 May 2021 01:18:15 GMT
RUN Set-PSDebug -Trace 2
# Tue, 25 May 2021 01:20:21 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 25 May 2021 01:20:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 25 May 2021 01:20:23 GMT
EXPOSE 4222 6222 8222
# Tue, 25 May 2021 01:20:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 25 May 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219fee2888f4047f4ac3a8210c73b803c05d01ea4b32fdd5885a96cf7ed455fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7979155d12f8cdfad103fe33a974b9b7a23eda3f84b01e6e810cfa879cc29bdd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6d5581c74b775110854326feb9ac80620ec010ba8fe3f766aa6d54c772c1fd`  
		Last Modified: Tue, 25 May 2021 01:22:06 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3870e6fcc58037755279cd186f632f2ccd83e01549e1b3d12b0632aba656d65`  
		Last Modified: Tue, 25 May 2021 01:22:12 GMT  
		Size: 5.7 MB (5701056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bf3ccaf0b4516bec19e9968499f60226dd228eaa038451ba1bb303169fb70a`  
		Last Modified: Tue, 25 May 2021 01:22:20 GMT  
		Size: 14.5 MB (14461027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4882198ee38c39e94a6ae9cd62261f7e8905481ab1383e8bfff483a0bda4ed`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 2.0 KB (2004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c6dd3b49ff2c29728aced07302b0d713312f70a0877cc9f508a9db4106b337`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8e4b0d0c2d782a3e477e196ccde922bd28752d07147ef304da3f8d70780193`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b816c180aed01b5f479de14fe796a664ea0f1bf45e768edab5dc11965d067a84`  
		Last Modified: Tue, 25 May 2021 01:22:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
