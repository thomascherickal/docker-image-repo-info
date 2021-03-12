<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.12`](#nats2-alpine312)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.1`](#nats21)
-	[`nats:2.1-alpine`](#nats21-alpine)
-	[`nats:2.1-alpine3.12`](#nats21-alpine312)
-	[`nats:2.1-linux`](#nats21-linux)
-	[`nats:2.1-nanoserver`](#nats21-nanoserver)
-	[`nats:2.1-nanoserver-1809`](#nats21-nanoserver-1809)
-	[`nats:2.1-scratch`](#nats21-scratch)
-	[`nats:2.1-windowsservercore`](#nats21-windowsservercore)
-	[`nats:2.1-windowsservercore-1809`](#nats21-windowsservercore-1809)
-	[`nats:2.1-windowsservercore-ltsc2016`](#nats21-windowsservercore-ltsc2016)
-	[`nats:2.1.9`](#nats219)
-	[`nats:2.1.9-alpine`](#nats219-alpine)
-	[`nats:2.1.9-alpine3.12`](#nats219-alpine312)
-	[`nats:2.1.9-linux`](#nats219-linux)
-	[`nats:2.1.9-nanoserver`](#nats219-nanoserver)
-	[`nats:2.1.9-nanoserver-1809`](#nats219-nanoserver-1809)
-	[`nats:2.1.9-scratch`](#nats219-scratch)
-	[`nats:2.1.9-windowsservercore`](#nats219-windowsservercore)
-	[`nats:2.1.9-windowsservercore-1809`](#nats219-windowsservercore-1809)
-	[`nats:2.1.9-windowsservercore-ltsc2016`](#nats219-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.12`](#natsalpine312)
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
$ docker pull nats@sha256:fd871c2d9cfc84d15900d6a66bb9e560ae784483035331414bdeacf4fe88686b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.12`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.12` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:8189f598985ffbfbad8d1f49a6369c85192e752d2f0c634e3814fd7266e981c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:d79c5ce5e1f64c5bcfcb75e557867e4bf0d46ba2975a35f2d653a1b9e8de4b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:fc0e60009c5d72028223e66ed67396b935dbfd43b83f7cdb41549190e57bf68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1`

```console
$ docker pull nats@sha256:fd871c2d9cfc84d15900d6a66bb9e560ae784483035331414bdeacf4fe88686b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-alpine3.12`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-alpine3.12` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-linux`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-nanoserver-1809`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-scratch`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore`

```console
$ docker pull nats@sha256:8189f598985ffbfbad8d1f49a6369c85192e752d2f0c634e3814fd7266e981c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.1-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:d79c5ce5e1f64c5bcfcb75e557867e4bf0d46ba2975a35f2d653a1b9e8de4b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:fc0e60009c5d72028223e66ed67396b935dbfd43b83f7cdb41549190e57bf68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9`

```console
$ docker pull nats@sha256:fd871c2d9cfc84d15900d6a66bb9e560ae784483035331414bdeacf4fe88686b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1.9` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-alpine`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-alpine3.12`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.9-alpine3.12` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine3.12` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine3.12` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-linux`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-nanoserver`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1.9-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-nanoserver-1809`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1.9-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-scratch`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.1.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-windowsservercore`

```console
$ docker pull nats@sha256:8189f598985ffbfbad8d1f49a6369c85192e752d2f0c634e3814fd7266e981c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.1.9-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.1.9-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:d79c5ce5e1f64c5bcfcb75e557867e4bf0d46ba2975a35f2d653a1b9e8de4b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.1.9-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.1.9-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:fc0e60009c5d72028223e66ed67396b935dbfd43b83f7cdb41549190e57bf68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.1.9-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.12`

```console
$ docker pull nats@sha256:bedd1037daa9e0098bcb7876d1888273dce87bbfba67b43b9ef91a05b76ffc93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.12` - linux; amd64

```console
$ docker pull nats@sha256:7ce5c7b565a5ded2ac499264f6619fa864126a6c086cacd0cfbecd8f6c354ece
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7178961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1589771fc3a21d4e9d1384531f1292dc189ea65e4180d50a781d05e0c92c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:17:47 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 21:17:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 21:17:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 21:17:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 21:17:50 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 21:17:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:17:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04da70183f3d4c74fd2a935bc17934825e90d3534658232dfde39ab25e28dc1d`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 4.4 MB (4378526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39e8336ba67bacd19b15b840b0b1c30f7dc0b84e7aecb628a4d5759b939246f`  
		Last Modified: Wed, 24 Feb 2021 21:18:27 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f624d5b3950c736fa499b7405fd8ce9856e27bf98654789f160f05a0cfe7d15c`  
		Last Modified: Wed, 24 Feb 2021 21:18:28 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.12` - linux; arm variant v6

```console
$ docker pull nats@sha256:182f983642f751c82ae4f9b0100e5a80e1b28e05eda71b2e3065a257552ed73d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6704726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0678de7fcb32a879700b60fa0da0cda23f94ff4d38070f6109972745f9f110a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 00:31:50 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 00:31:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 00:31:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 00:31:59 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 00:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 00:32:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb263be62fb2a203ab14e339c00d471f4a002bc8f58511c3decbb9fbfb2077`  
		Last Modified: Thu, 25 Feb 2021 00:32:50 GMT  
		Size: 4.1 MB (4099238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25e6c24534f913c9c5554f983b54d38e01b9aca0cb62d428afddcebc4e738d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e96fc1ca78459475e2fb21d62da2418ba801a21704ff3df9e16a205747f3d`  
		Last Modified: Thu, 25 Feb 2021 00:32:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.12` - linux; arm variant v7

```console
$ docker pull nats@sha256:b8db0408fafbd7b9e4837205e930e1d191a97d048443e1e32e5cc3f30d89b3a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6503692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6929a4291fc38f4391ae595a421fcb03148dd51263bf48e9b7ae24a5b84b4a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 21:03:35 GMT
ADD file:2632f48dd643f8927da2b1af8365b3edb484bd6b7d9fee4009e69f6cf3310e91 in / 
# Wed, 24 Feb 2021 21:03:36 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:01:03 GMT
ENV NATS_SERVER=2.1.9
# Thu, 25 Feb 2021 02:01:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 25 Feb 2021 02:01:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 25 Feb 2021 02:01:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 25 Feb 2021 02:01:19 GMT
EXPOSE 4222 6222 8222
# Thu, 25 Feb 2021 02:01:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:01:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8e85c7428c31ea48b47424ca0e4663106c54591c83545d32b66a77093f90ffd0`  
		Last Modified: Wed, 24 Feb 2021 21:04:23 GMT  
		Size: 2.4 MB (2408004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcee9fe1e23a6ccb2d96e8acf3ccf7dc882c1c4a6ecff19220e0ee873681c5f`  
		Last Modified: Thu, 25 Feb 2021 02:02:19 GMT  
		Size: 4.1 MB (4094717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0a0ce0771945aa06bce7f7614e821ee7af6bf92ec0a82f47bc833dad83c64f`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9210b7ab1af2ef08e109d0ed4e7081f821ffc27fb95643d236ae15fc1697b0`  
		Last Modified: Thu, 25 Feb 2021 02:02:14 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.12` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7e021a80389f3a50ac2ef5a74612013657976d59ac0feb5d07ed9097886edd74
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6789653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c302a5529d14e03c54164fb5441fdcbc211e7c9ef7a7c9a95ba6cf44fc3a2136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:39:21 GMT
ENV NATS_SERVER=2.1.9
# Wed, 24 Feb 2021 23:39:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='22659ec3653a2db53294427c8ec939a3b9d207a36ea54daf945b9fa43477434d' ;; 		armhf) natsArch='arm6'; sha256='761d1062303e9637196ab3b329d01609ea907d297e6c10f6932212b62ff9b1b4' ;; 		armv7) natsArch='arm7'; sha256='0a000c41c5031969f7b855cf4c65d5e6b1d6cd2230857f728a190a6ee128828c' ;; 		x86_64) natsArch='amd64'; sha256='c9538f4a47ffe75d11f3c5ce1e1c9a3c6ae1e26e26f7a1428ca5dda6b1b476d1' ;; 		x86) natsArch='386'; sha256='079cbfc5f42ebbe2b696fdc88c75ffdebd3b9f34e88d61a829ced064ab48a749' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 24 Feb 2021 23:39:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 24 Feb 2021 23:39:27 GMT
EXPOSE 4222 6222 8222
# Wed, 24 Feb 2021 23:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:39:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6157226fdda6773a389fc34c20d497af9c6528f070c597bd838d964f5a8ce5`  
		Last Modified: Wed, 24 Feb 2021 23:42:41 GMT  
		Size: 4.1 MB (4078803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d5a5f9b7b6184a92bff656f27feb392e19994cc96309ae38888c1036899648`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d11eec2698149186fe044feab773d9971fd08e7f15ad892950bdd59702b60e`  
		Last Modified: Wed, 24 Feb 2021 23:42:40 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:fd871c2d9cfc84d15900d6a66bb9e560ae784483035331414bdeacf4fe88686b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:89252c4696decba3dc5ceeffa42c97c91e19d28f1ba15b3cd6dd6dcb6e5540ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:920d8ade1a4f6d90695652a4349fb6eece54f8360f64ed8dcf76163c000cfb36
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105438714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0fab6cf3c68ad9f23a7f7dc02d2649d460096af3b7a9ea4f092b9d7e500f3c7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:56:56 GMT
RUN cmd /S /C #(nop) COPY file:1bed18dba32dca3cc37e8d20c1b6b2b5179bbc92f869531591951b440efda07a in C:\nats-server.exe 
# Wed, 10 Mar 2021 16:56:57 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:57:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a316d8907eb48fc6b8f80a4bf7ed9f4edf301f82dcd805b18a5064f8258a53`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 4.0 MB (4042849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb866ffe49554061a3211989b4d25bcea6fb80039d53ad8c9c3c68ba4fda4e81`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.6 KB (1646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29614a926fb02cda335c6d1478db8b216e6702ba39526930932efceae76e189a`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fda256d1eb52527f059b59a10da53a6ecf210ded5ff15a503d604763d18b12`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7513c896811523a609b634b4dce25d6f4369948818c1b34d4a978031172391d7`  
		Last Modified: Wed, 10 Mar 2021 17:01:55 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:dc0ba254275cb917eec2b9d1fd1055fe132c854a9afea39628c4871a10b49db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:679524b91e0a1e4b983d20d70f7a1495f1c16247cf568f29cbf88f5c4b25e914
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4098136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95713166e2236aefedbb92b1d1ef989f979e5c737ff5c14d45d9e32803f032bb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:e0a0cbd14b84d81f9a3d73a7eefe99693215eb890370f9aba1b574d4cbf63b52 in /nats-server 
# Tue, 03 Nov 2020 00:32:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:32:03 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:32:03 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:32:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2d6c7151b0c792ecf790fde24412769bf193e4c1922c8a508f8e137d292b4179`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 4.1 MB (4097661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b920bf257e35e5e325af3ffc17a4baed7903a77f327e8ec3021f94016a78a239`  
		Last Modified: Tue, 03 Nov 2020 00:32:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7c6e8cffea7e48d3ee02b22fb93947963731051dcc56f3c8ec98f2260768814b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3817067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a584107a14f067c0a007db6f0e42b3ff0c190fa2d866f5581552cc559a035125`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:4cd9814103fc39d1b5bf81e4e528b12e56d59d0efda223c50a7ea420e6d4b421 in /nats-server 
# Mon, 02 Nov 2020 23:53:40 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 02 Nov 2020 23:53:41 GMT
EXPOSE 4222 6222 8222
# Mon, 02 Nov 2020 23:53:41 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 02 Nov 2020 23:53:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e162374a08bbb575088c1eaffc753891ab6589b134493a9f8ba1b148e20f8dec`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 3.8 MB (3816591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77a00778e9ed2ae19795da75b6f12f291e70490f03cc4565c407af242ace47`  
		Last Modified: Mon, 02 Nov 2020 23:54:20 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:1f4b725d1989c235e10f362b0f9c04a708fe6b1dfb22e2efc236b0d2a001ef8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3813415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483d6781ef03c3263effcb9f73ae01394a0dae4af477e75c00c19544d0bfe66b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:0513d05e9f97918c0430b076865e30771904270865892c092e15d1beb98d08c4 in /nats-server 
# Tue, 03 Nov 2020 00:03:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:03:53 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:03:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:03:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ed0e6ae1888bfc5be9efcd3bbca71bd2840e4361003c98476fd25ce7d6e9ee14`  
		Last Modified: Tue, 03 Nov 2020 00:04:34 GMT  
		Size: 3.8 MB (3812940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b242a83395577c4be465d49aee9b3d407ea026cb0383e18836fb6ed16caa34c`  
		Last Modified: Tue, 03 Nov 2020 00:04:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:670bb4f03b559b3f9d0d2e736450bbb77ae1a789bbfac3b11a09c531d6cf412e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3795291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd733d2cc8ad31f06df9779323962d0e6f73681100397d3090b1e57bc25be709`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:e1e30af7043f9127562e3a3ea4612aaf12d52aac32a8466b822dbbbeebaaef76 in /nats-server 
# Tue, 03 Nov 2020 00:21:37 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 03 Nov 2020 00:21:38 GMT
EXPOSE 4222 6222 8222
# Tue, 03 Nov 2020 00:21:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 03 Nov 2020 00:21:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6433bc19867b0af777bb4176a307bfb021a5ee3d3ad8390bb912e6787b729c8`  
		Last Modified: Tue, 03 Nov 2020 00:22:16 GMT  
		Size: 3.8 MB (3794815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d0ed92b996d8a726daa5da839bd0dfa4651c38c36a2f9a62af31ed304b10a6`  
		Last Modified: Tue, 03 Nov 2020 00:22:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:8189f598985ffbfbad8d1f49a6369c85192e752d2f0c634e3814fd7266e981c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:d79c5ce5e1f64c5bcfcb75e557867e4bf0d46ba2975a35f2d653a1b9e8de4b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:8ffbbc19fc787cd97ef4382c6d7acae1ef7aab53f8fc7299ea222b37b1a7df33
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480073345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e5e56416ebe2e81ec1efe2eca5ddbed45e6c8fe76ab4dbe5f6956afddcdee7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:54:56 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:54:57 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:54:58 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:55:29 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 16:56:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 16:56:43 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 16:56:44 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 16:56:45 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 16:56:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cef1f35e24b14a5d662b81a0a554ccfedc57f0d3a038a11e35356b073c1b5c`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316c63e2571e239224f25e77f14564870d0a4a8d3af4eee9931f3f0c17a6aec1`  
		Last Modified: Wed, 10 Mar 2021 17:01:36 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2658e07d6f43ab6d2872ad27694424a15f699d085b8402975422e719e615684`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ad6be90721126d6eb5acc637d22ae2edbc998755169ee145ffd47001374980`  
		Last Modified: Wed, 10 Mar 2021 17:01:35 GMT  
		Size: 5.1 MB (5064780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc89af611cb21d10d62a05ae09af65d108327328dc2e4e8389271c545b7d88`  
		Last Modified: Wed, 10 Mar 2021 17:01:34 GMT  
		Size: 13.5 MB (13461502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0715724ff8d8c9176d4b6d33f92788befd97f0c54d6bcd72d4cc78c2d7a470da`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.9 KB (1942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c5363d54ca6b3865aaf2bd95ea933ee7e5ee79d4ddcc10b4cf83cff00174aa`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca21cdce5760d97af5f9acb1d2f024098a5ab148f073ecc3bbbbeebafe2bf859`  
		Last Modified: Wed, 10 Mar 2021 17:01:30 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434bb22e43e84693524439412a3f2de76de2ff15ed4cdf792b2e9b79e872d027`  
		Last Modified: Wed, 10 Mar 2021 17:01:32 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:fc0e60009c5d72028223e66ed67396b935dbfd43b83f7cdb41549190e57bf68b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:66126fdcc8018d2d2f9fbe281188a56efbb436849eb06ce5e2c181eeaa9b619b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816773837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad00d7822043d66e214b8523e52b7beb31d15c68c58cb98c362223663fe7d911`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 Mar 2021 16:57:10 GMT
ENV NATS_SERVER=2.1.9
# Wed, 10 Mar 2021 16:57:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.9/nats-server-v2.1.9-windows-amd64.zip
# Wed, 10 Mar 2021 16:57:12 GMT
ENV GIT_DOWNLOAD_SHA256=cb4ec25356a0200edcd5df579cfa06154f5576c2c48d3727dca2117d6e7e5891
# Wed, 10 Mar 2021 16:58:32 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 Mar 2021 17:00:28 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 Mar 2021 17:00:30 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 10 Mar 2021 17:00:31 GMT
EXPOSE 4222 6222 8222
# Wed, 10 Mar 2021 17:00:32 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Mar 2021 17:00:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58c165493987dd29c1c0acacaf9c0ff15a557060f1848ea26996b9ce21aae0`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78982f85c559dbd12ee3f51b834a0ef77c43acb0f1fff24faf9e389631b96c`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f0d273c80c1dbd9b8813a188e5920191ce2507e40d0350ee441ec34a3e9e3`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5453b687f1986b2e87d86225d728a9feb743157f8cb566b9c1d6d0ce58110e`  
		Last Modified: Wed, 10 Mar 2021 17:02:26 GMT  
		Size: 5.6 MB (5647961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca39166547ab6aa791b61b8180813822efc34d6f57b9c72f1edacacaa8bac2`  
		Last Modified: Wed, 10 Mar 2021 17:02:20 GMT  
		Size: 14.2 MB (14202739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0deae7874091de5a817595e8a5924980e12a421f9d28832257fdad32a4e3f0`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.9 KB (1855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2fd64751fb1de794b023f59afed0f96ade2d01ddf5dc5f7b58a2688b7b611`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cbeb30ccb829bb2bd06131b3cc0a0b9963ad6c19a65c8ad9f9f7cc8a2f609e`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ab7b94c330f979e9c58deccfd61c87f8ab16f439585082237f3f8a83e924aa`  
		Last Modified: Wed, 10 Mar 2021 17:02:17 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
