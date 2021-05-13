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
-	[`nats:2.2.4`](#nats224)
-	[`nats:2.2.4-alpine`](#nats224-alpine)
-	[`nats:2.2.4-alpine3.13`](#nats224-alpine313)
-	[`nats:2.2.4-linux`](#nats224-linux)
-	[`nats:2.2.4-nanoserver`](#nats224-nanoserver)
-	[`nats:2.2.4-nanoserver-1809`](#nats224-nanoserver-1809)
-	[`nats:2.2.4-scratch`](#nats224-scratch)
-	[`nats:2.2.4-windowsservercore`](#nats224-windowsservercore)
-	[`nats:2.2.4-windowsservercore-1809`](#nats224-windowsservercore-1809)
-	[`nats:2.2.4-windowsservercore-ltsc2016`](#nats224-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:1e73835df48665074bbfe2d19c82563c6adc3ee0fcdd5b40a98e6722a3e9959d
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
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:3d54f8ea39c1289fcdeb4030e57a26e16066bcc68a8bf5b1665764324b22d6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:1c4b5d77226f0ba6b8e0c4d2e6984042fb44ca4f17225a682035b797242ff2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:bba033611034c965ca7d6847f4633a856da117d106d76544795f4dd2baeb8cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:1e73835df48665074bbfe2d19c82563c6adc3ee0fcdd5b40a98e6722a3e9959d
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
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:3d54f8ea39c1289fcdeb4030e57a26e16066bcc68a8bf5b1665764324b22d6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:1c4b5d77226f0ba6b8e0c4d2e6984042fb44ca4f17225a682035b797242ff2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:bba033611034c965ca7d6847f4633a856da117d106d76544795f4dd2baeb8cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4`

```console
$ docker pull nats@sha256:de009186c4dbf527f3fb2272ae74ef302256ebc70a1876df15986455f6218229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.4` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4` - linux; arm variant v6

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

### `nats:2.2.4` - linux; arm variant v7

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

### `nats:2.2.4` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4-alpine`

```console
$ docker pull nats@sha256:f1b4201ad785b76e568c68f4ed17c3dd0715e006dfa1cc15b094071e3719762d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.2.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4-alpine` - linux; arm variant v6

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

### `nats:2.2.4-alpine` - linux; arm variant v7

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

## `nats:2.2.4-alpine3.13`

```console
$ docker pull nats@sha256:f1b4201ad785b76e568c68f4ed17c3dd0715e006dfa1cc15b094071e3719762d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.2.4-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4-alpine3.13` - linux; arm variant v6

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

### `nats:2.2.4-alpine3.13` - linux; arm variant v7

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

## `nats:2.2.4-linux`

```console
$ docker pull nats@sha256:47f14fbac1bbce32c5d3a2307287e52859d076f5d455a55292670932a8dbe78f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.2.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4-linux` - linux; arm variant v6

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

### `nats:2.2.4-linux` - linux; arm variant v7

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

## `nats:2.2.4-nanoserver`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.4-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4-nanoserver-1809`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.4-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4-scratch`

```console
$ docker pull nats@sha256:47f14fbac1bbce32c5d3a2307287e52859d076f5d455a55292670932a8dbe78f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7

### `nats:2.2.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4-scratch` - linux; arm variant v6

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

### `nats:2.2.4-scratch` - linux; arm variant v7

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

## `nats:2.2.4-windowsservercore`

```console
$ docker pull nats@sha256:3d54f8ea39c1289fcdeb4030e57a26e16066bcc68a8bf5b1665764324b22d6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.4-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.4-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:1c4b5d77226f0ba6b8e0c4d2e6984042fb44ca4f17225a682035b797242ff2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.4-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:bba033611034c965ca7d6847f4633a856da117d106d76544795f4dd2baeb8cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:0033d37a01d3de45800b65a6c4cdf355dd0159c93685eabcbdfd344e201d4849
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:6cf526eed3659edaa3b26d1053fddf373daa8145465d06975af2a5abef2f72ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7339184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e988e425667d44a3e6a92fdc586e719ca7e7d34d6101b6cd700b927be2f22a59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 13 May 2021 18:20:07 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:20:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='88ad3d5fbef04ad3298ab528a1dc59f8531e313a0b47dc39606d8fbe29e71341' ;; 		armhf) natsArch='arm6'; sha256='cbcf6db915022c723149b609706d5fcf87f02ddca1c0dd0367870e394005b89d' ;; 		armv7) natsArch='arm7'; sha256='80be30d9caba8aa4661ed50fe64eeb454ff023f54a3687b85293f55bf6725d33' ;; 		x86_64) natsArch='amd64'; sha256='419b3a8761d1120c40851e2ac6d820695ca6b300e95933d88603cbd1255043fa' ;; 		x86) natsArch='386'; sha256='fd82800d141072f27f2c9e34ac287b40b3f086be4dca5a159611ce0e03f04ec2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 13 May 2021 18:20:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 13 May 2021 18:20:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 13 May 2021 18:20:11 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 13 May 2021 18:20:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217a0b59da619835f01da5a589ed121081784a8917fb99e3733e136b01b0b2e`  
		Last Modified: Thu, 13 May 2021 18:21:27 GMT  
		Size: 4.5 MB (4526242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7631199270cbaad4a3fc4ac4af1359e22a1d76fe6f0abd5d3116219dd6e0a125`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448706151ceb4a7313a8f2bb4df5e1868ff7e0709ada7295d2f258fe258cca59`  
		Last Modified: Thu, 13 May 2021 18:21:26 GMT  
		Size: 415.0 B  
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
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:1e73835df48665074bbfe2d19c82563c6adc3ee0fcdd5b40a98e6722a3e9959d
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
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:10cdbe8b77248b0dc115ccceaadeab601fd2645d6d141e56a6c660dabb9cb7b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:e1ca9851a80bcb55f85eff4d11ea76149217703c40b568e6d22b232c09f86a6a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105681386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b768b6d1ad37b5a86d65cc0c778a033149bcbf5d3a4bbb35af889718c499c04a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 13 May 2021 18:17:34 GMT
RUN cmd /S /C #(nop) COPY file:6770dfb1874ec9c6166c8748998bb42df4205ff12bf6f7274d60feb7648dcd48 in C:\nats-server.exe 
# Thu, 13 May 2021 18:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:38 GMT
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
	-	`sha256:82ac98db28638663f44c408e552c9beb39d8e97bc57459afc9f258e0d7874034`  
		Last Modified: Thu, 13 May 2021 18:22:52 GMT  
		Size: 4.3 MB (4299702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c80b8f59e6a483e1a194ba34cddb4fc91ded64bb9cafa5dfce277775df7b7`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.8 KB (1778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdeab49db11bf9bdd57979065493223304ca04e1badf1cbce1393967c8f7ede`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505de34e9f545d6f8d9e014fb64b78b48aceb393b3b50e2eafc7fea4054fe003`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b7564633657b5e2012d7f76e6f0b6d092b588718aff2db3e67af03892eafe`  
		Last Modified: Thu, 13 May 2021 18:22:51 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:2a3f30710d699f2bd1d5cf48e793da62e00660f59a3955911e3dd721d326e775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:5c1e54ae38b51513897faa4e9026b4604e7aa4564476494191577e2c4cbcf49d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4244330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec16f317835a6c61c09b94494fad37939256a04d1fb9081fba712630a879e79f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 13 May 2021 18:20:59 GMT
COPY file:56b7cb01b12b627a78f83c55a73796427b54e159964a79e9180a50239e4f7390 in /nats-server 
# Thu, 13 May 2021 18:20:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 13 May 2021 18:20:59 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 13 May 2021 18:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da7b6c6e1ed51e69f2d6201433db9ea9b65ecfe27c6aaf70e6fab7763cc1fc43`  
		Last Modified: Thu, 13 May 2021 18:21:53 GMT  
		Size: 4.2 MB (4243853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ca532024f2853525c46d903e0ac66f7eeed5b4c94a6a4a8872fef94f1dca3a`  
		Last Modified: Thu, 13 May 2021 18:21:51 GMT  
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
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:3d54f8ea39c1289fcdeb4030e57a26e16066bcc68a8bf5b1665764324b22d6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:1c4b5d77226f0ba6b8e0c4d2e6984042fb44ca4f17225a682035b797242ff2aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:f23d476edf63ab9ffb2d92a12a75c014440212217f595337cf3b9558feba8d23
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488965465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2173bd97e00e6eaff464688f0e73f6d09d315fba5cb04ba626a071a9666345fa`
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
# Thu, 13 May 2021 18:15:21 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:15:22 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:15:23 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:15:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:17:14 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:17:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:17:16 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:17:17 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:17:19 GMT
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
	-	`sha256:aa8c985fbc1c7f8c2501d1fab48cd4dd4bbf2b53917a99dd224bf0fd98807c4a`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96c03f261eb3a4ab917194a72941aaef4c63720f6074be26a7d538e0fdf9c20`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf57f2b1747bc26fd7bb9bfb8c1528d5b31fbed2b641b6b6d3e46a1947a005d`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80464502fd0798acc0e2890d69faf460191cf90531c065e51649a4504a45e71`  
		Last Modified: Thu, 13 May 2021 18:22:33 GMT  
		Size: 5.1 MB (5097311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7494e06648bff82ed2645ef7858d7fc192158ecd2a7199c19d65fd96f83c598`  
		Last Modified: Thu, 13 May 2021 18:22:27 GMT  
		Size: 9.4 MB (9365665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea83d11264df7650072aad270a91055d704bd12325c1acea9960cd21b426e26e`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 2.0 KB (1957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87db3c8226085de0d9e4a77fff18214da4c10dfe72fef5e65d72bfd7b90a93d`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c523b4566a067c1a9984ad2dfe99480d98eba839d5a03e3d25e0a78812e647d5`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de5cc7439f204d66c2da12ecd3fd30d6d892bad2e108d22e8bd3f1d3b163a7`  
		Last Modified: Thu, 13 May 2021 18:22:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:bba033611034c965ca7d6847f4633a856da117d106d76544795f4dd2baeb8cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:7647918261d11c4129e46342b5ead2bd4a7fe5890a1eabc4c8bc15117a6aafdb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815985063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8351132feba4c7211a1c6494d5aad2d2feca30b631c5c27869149ceae39308cb`
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
# Thu, 13 May 2021 18:17:48 GMT
ENV NATS_SERVER=2.2.4
# Thu, 13 May 2021 18:17:49 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.4/nats-server-v2.2.4-windows-amd64.zip
# Thu, 13 May 2021 18:17:50 GMT
ENV GIT_DOWNLOAD_SHA256=fd0a68ebbd0225bfa30981699c9b5de3e0bb21db7eacbde7772021cd39cf7d7f
# Thu, 13 May 2021 18:19:26 GMT
RUN Set-PSDebug -Trace 2
# Thu, 13 May 2021 18:21:33 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 13 May 2021 18:21:34 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 13 May 2021 18:21:35 GMT
EXPOSE 4222 6222 8222
# Thu, 13 May 2021 18:21:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 13 May 2021 18:21:38 GMT
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
	-	`sha256:c50e486f7d07050146376fe817fbaa36684d4a4c92ba71ce2493904b8e971627`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dfc4c4856991011c03cb36f66e5603195775041170086e915179ae447f12b`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1721d0ded1eec67890352a406e6b14542008bd9e4ab391d56b630212225c21`  
		Last Modified: Thu, 13 May 2021 18:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d2310fc7f04c4bfa4f3d8c209415d3c4d2e370bcafc6783ac0cb68372df0fd`  
		Last Modified: Thu, 13 May 2021 18:23:13 GMT  
		Size: 5.7 MB (5700657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a505b878f376494baa36819bde8e2ab831b07984e236dd7ecc89ceef04ac5fd`  
		Last Modified: Thu, 13 May 2021 18:23:12 GMT  
		Size: 14.5 MB (14493751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3a5995380bec58fd2f51e5fea55c90abf06ed3fad947ccbee69af0db0728b2`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7058f8afc5efca9f3c7c6958a56aef67b654759c9b1eee80cd7ccd64dca19f29`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70901d0156f2610812331f6382df909c63e125fc2e7170237b34bd4f775feb5`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a85a17ae63e3021a02ae1cd64d1f9c0a1aa8f3c5fedc6c3251caa5c9f98974`  
		Last Modified: Thu, 13 May 2021 18:23:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
