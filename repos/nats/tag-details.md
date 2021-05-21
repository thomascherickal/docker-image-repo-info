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
-	[`nats:2.2.5`](#nats225)
-	[`nats:2.2.5-alpine`](#nats225-alpine)
-	[`nats:2.2.5-alpine3.13`](#nats225-alpine313)
-	[`nats:2.2.5-linux`](#nats225-linux)
-	[`nats:2.2.5-nanoserver`](#nats225-nanoserver)
-	[`nats:2.2.5-nanoserver-1809`](#nats225-nanoserver-1809)
-	[`nats:2.2.5-scratch`](#nats225-scratch)
-	[`nats:2.2.5-windowsservercore`](#nats225-windowsservercore)
-	[`nats:2.2.5-windowsservercore-1809`](#nats225-windowsservercore-1809)
-	[`nats:2.2.5-windowsservercore-ltsc2016`](#nats225-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:e7196d68027c9d81fd783b689c81bd8f9ba32b400088c2a3652a606855530eb4
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
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:6343e22445146a2e0ab15ff6e168f12d7ab9074d12819efc96856ba91d355cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f3ea4c55909d3b260e1d6a640115c42ebc240f0c6287bb0e355a0021698ca24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f5e1a7a908d5beaecc090e7ca32ddf92f1e7b3d646ebf82cc260ba78a1bd27a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:e7196d68027c9d81fd783b689c81bd8f9ba32b400088c2a3652a606855530eb4
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
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:6343e22445146a2e0ab15ff6e168f12d7ab9074d12819efc96856ba91d355cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f3ea4c55909d3b260e1d6a640115c42ebc240f0c6287bb0e355a0021698ca24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f5e1a7a908d5beaecc090e7ca32ddf92f1e7b3d646ebf82cc260ba78a1bd27a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5`

```console
$ docker pull nats@sha256:8bcffe2ec8efe43864321bffa5285bc8d5493018a6d60adc952ba86953ca1c94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.5` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.5` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-alpine`

```console
$ docker pull nats@sha256:a310de5d750e0ced27eff899c58d6ea3dac1831c54a1f5bbddd2a4fc5df06652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `nats:2.2.5-alpine` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-alpine3.13`

```console
$ docker pull nats@sha256:a310de5d750e0ced27eff899c58d6ea3dac1831c54a1f5bbddd2a4fc5df06652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `nats:2.2.5-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-linux`

```console
$ docker pull nats@sha256:c76ab47b4cbbabf4a9b81570cd6834d0612f2ff78a55ccd2259384e9c8b99d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `nats:2.2.5-linux` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-nanoserver`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.5-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-nanoserver-1809`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.5-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-scratch`

```console
$ docker pull nats@sha256:c76ab47b4cbbabf4a9b81570cd6834d0612f2ff78a55ccd2259384e9c8b99d3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `nats:2.2.5-scratch` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-windowsservercore`

```console
$ docker pull nats@sha256:6343e22445146a2e0ab15ff6e168f12d7ab9074d12819efc96856ba91d355cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.5-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.5-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-windowsservercore-1809`

```console
$ docker pull nats@sha256:f3ea4c55909d3b260e1d6a640115c42ebc240f0c6287bb0e355a0021698ca24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.5-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.5-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f5e1a7a908d5beaecc090e7ca32ddf92f1e7b3d646ebf82cc260ba78a1bd27a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.5-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:6cf3cec87b97bc4869de88dda543bd1c400ccb9521c7aef36d33a99d515c0ce1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:05f0c41f3164ca644d2bb64afe5b19e6a1850b9cf533746cf91bd9aba605f6e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7343161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5bcc5fe6b13327458c8febb3c390c500da37308da3903843de364de6a2ce554`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Fri, 21 May 2021 01:20:29 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:20:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='12f06d3ac1af3872c8b77722e19faa508b979806641a6dc2707f641de270aa49' ;; 		armhf) natsArch='arm6'; sha256='a61769ab4f4176c882a69209bbff54e0e7e8bd6e986ba8841d5a061a4f8cc72f' ;; 		armv7) natsArch='arm7'; sha256='307b3a42492a0a0172df5d00dea3355064daf5cf38653a1835fab39ca0393415' ;; 		x86_64) natsArch='amd64'; sha256='e4f57f263c7411f6028e9cd6080c6fd35090de4168c21c3e8b7a5ee5a632d142' ;; 		x86) natsArch='386'; sha256='fd3025f88aca3e89d1015d5d3aedfd9390146b168703e2777616261bcc752e2c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 21 May 2021 01:20:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 21 May 2021 01:20:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 21 May 2021 01:20:32 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 May 2021 01:20:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4ca912af8a523a4d5305fc703d6103e03f3994bccd440e31ede887688be714`  
		Last Modified: Fri, 21 May 2021 01:21:23 GMT  
		Size: 4.5 MB (4530220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108976c3e63e0003f5e4d5ed04bf985f6ac7f46826a9f2099ceb572d9e88cb0`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f907db8c0f6fef0f88ecb1319563866ac55ba7dc88a4d4b94a624ccb9896efe6`  
		Last Modified: Fri, 21 May 2021 01:21:22 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:b3c5544c5b1d2029e036dc2d81c5ef9a9eac93c249716e18f44edef627978f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6614265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f522cda51f5777e741129fc6a3a6e6c829fd2ae89a356be63fa4d268fd59419d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 17:59:46 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 17:59:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 17:59:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 17:59:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 17:59:54 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 17:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 17:59:58 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7360a77507600c48adcac31f54a9378253c081d72935f0eae5e523bfd31b34`  
		Last Modified: Thu, 13 May 2021 18:07:02 GMT  
		Size: 4.2 MB (4189145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f603eb8e24e2c3c865dca1242b14eb6277a939d61d513679c8efc3d80a7a5373`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5013eb5a0ee908a4d4462e87197f966195cd787b7d3afe9392b7d36a3a2de10`  
		Last Modified: Thu, 13 May 2021 18:07:01 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e7196d68027c9d81fd783b689c81bd8f9ba32b400088c2a3652a606855530eb4
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
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:a51cf33b5a60f76e42ca151a63dcd64c5014d52741be152540b12678b5c5811d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:db6f507814fd84844ba385a380408a279d3437419ef81c7333b688939e40747f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105685386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64cad50065fed8d849cda0d7d7f8ad084f1850266def42da1967d0d574b05f5b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 21 May 2021 01:17:29 GMT
RUN cmd /S /C #(nop) COPY file:84543609fdaaa8bc52c8296374bbd0ecb12f7921f77a50ab92dd457e006d99eb in C:\nats-server.exe 
# Fri, 21 May 2021 01:17:30 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:31 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:32 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:33 GMT
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
	-	`sha256:d1f2f10620988c53d1413e1de64a803b287ca04340f5e3510fa30692ea487890`  
		Last Modified: Fri, 21 May 2021 01:22:42 GMT  
		Size: 4.3 MB (4303729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5f0a6a4b00d17ab7fab29536df846b23f6797e5b1b09d06a7611cec4f17a36`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a012d1dcfa8e2726551ffeee347ec08c0294fa8c8420b45169a643081f303735`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c511b3e18baf77860f1803c053ec04aed87b960783cb978d33959a43dde28d6`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d46e1fc180c8768dd3902fd3c7ee1cc4d98e5b2502b92c91c8c29cd8ab0f624`  
		Last Modified: Fri, 21 May 2021 01:22:36 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:aee27d05c4ddde1a2e00b42d643699a8d3d37c8433c85322eb20a9efc4c6334e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:abef0c3ba249694c80952bc78ca631eae41e1271fcd73c86e81fc4097c393c96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4247381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c3b84dc977adcc458f2f053d5fc6bd3295a18170b171ef6c62bf1f5d3a9608`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 21 May 2021 01:20:57 GMT
COPY file:fbdd1b7433eef5e551e3be723bab725d703c2614d47efe260ffecdfd5741ba8b in /nats-server 
# Fri, 21 May 2021 01:20:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 21 May 2021 01:20:58 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:20:58 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 21 May 2021 01:20:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6611569c04790370495ad267df6c2329dceeb4656aaa8ce0321c7d2a9987645f`  
		Last Modified: Fri, 21 May 2021 01:21:48 GMT  
		Size: 4.2 MB (4246904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee8df74c7ac110c48eb5d6bd0d0fe1979ad8ac3b6aa1d312eec39d6bd7e6f4a`  
		Last Modified: Fri, 21 May 2021 01:21:47 GMT  
		Size: 477.0 B  
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
$ docker pull nats@sha256:9eaf28be8f88c9b912476266f03838383b7e5060048f625bc5e7643f82deb26d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3910038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb219061a01dd4e1793c382cccb67984482ad879f1267ace4b4eeaf5b88fcc86`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:06:26 GMT
COPY file:951b0f900abe2121c3767e5b1a974baa8e184a53ac43db17a9cbb56d1e362fe7 in /nats-server 
# Thu, 13 May 2021 18:06:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:06:28 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:06:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:06:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c072ce563493afe1fd3c33e3283378af9b7d293dbbea9051ba5dac8fe7f1a86c`  
		Last Modified: Thu, 13 May 2021 18:07:18 GMT  
		Size: 3.9 MB (3909562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ee0f9f4512aca959a51df9c7b63048ab71fbbf40d77afbc460c1eaedeef`  
		Last Modified: Thu, 13 May 2021 18:07:16 GMT  
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
$ docker pull nats@sha256:6343e22445146a2e0ab15ff6e168f12d7ab9074d12819efc96856ba91d355cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f3ea4c55909d3b260e1d6a640115c42ebc240f0c6287bb0e355a0021698ca24e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:553ab1ce45bd46319b5725c4ea4de6b7dcc7f134a9b55e714e4cff3071a28f27
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2489015393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6db786d738e72eab560c58d9dbbd7cc94652b6b709df212c481bfd1ebe0e6122`
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
# Fri, 21 May 2021 01:15:17 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:15:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:15:19 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:15:54 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:17:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:17:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:17:14 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:17:15 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:17:16 GMT
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
	-	`sha256:4eacc1557a5f598517d44067ac8b634ea5d5e69d42a1617106f9917729a8c379`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa7e8f9ba961758d5a71af29a4a19cf6ca923af4448ae8a6277e1377d51f530`  
		Last Modified: Fri, 21 May 2021 01:22:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4079551a9fca404ec9047c7636afa519b4f3c0ce24ffba49c9d4503bb4b4fc1c`  
		Last Modified: Fri, 21 May 2021 01:22:10 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbead1c591568fa5311d9717df9a03bcbc282c2e69bca75ce29d267124440de7`  
		Last Modified: Fri, 21 May 2021 01:22:12 GMT  
		Size: 5.1 MB (5121053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379f226586f2c06e7a584a154bff396271b8bdeea8bb4aa2e8037d6026df831`  
		Last Modified: Fri, 21 May 2021 01:22:19 GMT  
		Size: 9.4 MB (9391861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5225325bfc14a5f9df997fb0fc74c89153de81b9b13ba8bc4cd5f540978d4c`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ab2c552e1b6e47aab0a8ea18011e429db83e3011e396d73a0c5b32b20996ba`  
		Last Modified: Fri, 21 May 2021 01:22:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cdaadb4db8cdde5c7cea375f57180c5d516d136932d10fd7c44e364a54c31`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db123c2d63b10aa6d21dd4071dfe6a32635e695067a54beb2a94a6a09297c24`  
		Last Modified: Fri, 21 May 2021 01:22:08 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f5e1a7a908d5beaecc090e7ca32ddf92f1e7b3d646ebf82cc260ba78a1bd27a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:af6a479ac67823cd29228d23d3fe797e8e009e9c1987aebfca481912f7db1bc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815986529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:109f28c28e9f87f8c0f69c42839e0a3f8636808c2e84027981406fc988afbe5d`
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
# Fri, 21 May 2021 01:17:43 GMT
ENV NATS_SERVER=2.2.5
# Fri, 21 May 2021 01:17:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.5/nats-server-v2.2.5-windows-amd64.zip
# Fri, 21 May 2021 01:17:45 GMT
ENV GIT_DOWNLOAD_SHA256=01ee2d426b856fb8729ade8a20d3f1ec16e4883b4c9bda02b76270fb0654848e
# Fri, 21 May 2021 01:19:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 21 May 2021 01:21:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 21 May 2021 01:21:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 21 May 2021 01:21:19 GMT
EXPOSE 4222 6222 8222
# Fri, 21 May 2021 01:21:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 21 May 2021 01:21:21 GMT
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
	-	`sha256:f0f3603b9524e93e5215c2abba5afdf68a7402c199c6044081404215e3ca09ed`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfaee8f415fdf30a7173aca01dd406a0dc11b64bf22445d8ba10838ab73f5cc`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba0596bf5825d8b175760cadb4aa03bc8bfff3cb41088d8bed50f495efc9974`  
		Last Modified: Fri, 21 May 2021 01:23:01 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933b94135b57dbf1dbc2823aae3e8c232d5078c506cc6ab357dd294fb8308187`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 5.7 MB (5699902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b118a826228e68680a9764693342bbf52ffb2c132cd3482c8235c8637efed1`  
		Last Modified: Fri, 21 May 2021 01:23:02 GMT  
		Size: 14.5 MB (14496050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61cf67042c8c5449c0e8f5baa07aec6e3907808d9c64e79d22e6bafa152b5ab`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 2.0 KB (1962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67754daf786179eff413898a2d98262cb69b817c93a7659504d2220af5727780`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067668e0d80f3d3321ce3cfdfdb3e4f901ff14219b46fc2d432115e97afc4cf4`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dc212c86917e270b694d1cd121320509bb1afa338b24c3d2d239dee1c19ad2`  
		Last Modified: Fri, 21 May 2021 01:22:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
