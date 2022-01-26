<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.15`](#nats2-alpine315)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.7`](#nats27)
-	[`nats:2.7-alpine`](#nats27-alpine)
-	[`nats:2.7-alpine3.15`](#nats27-alpine315)
-	[`nats:2.7-linux`](#nats27-linux)
-	[`nats:2.7-nanoserver`](#nats27-nanoserver)
-	[`nats:2.7-nanoserver-1809`](#nats27-nanoserver-1809)
-	[`nats:2.7-scratch`](#nats27-scratch)
-	[`nats:2.7-windowsservercore`](#nats27-windowsservercore)
-	[`nats:2.7-windowsservercore-1809`](#nats27-windowsservercore-1809)
-	[`nats:2.7.1`](#nats271)
-	[`nats:2.7.1-alpine`](#nats271-alpine)
-	[`nats:2.7.1-alpine3.15`](#nats271-alpine315)
-	[`nats:2.7.1-linux`](#nats271-linux)
-	[`nats:2.7.1-nanoserver`](#nats271-nanoserver)
-	[`nats:2.7.1-nanoserver-1809`](#nats271-nanoserver-1809)
-	[`nats:2.7.1-scratch`](#nats271-scratch)
-	[`nats:2.7.1-windowsservercore`](#nats271-windowsservercore)
-	[`nats:2.7.1-windowsservercore-1809`](#nats271-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.15`](#natsalpine315)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:3ac4fc48a5f45ba948539c44528787c6a0e278075b638ae32db2f5ea8567d76a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7`

```console
$ docker pull nats@sha256:3ac4fc48a5f45ba948539c44528787c6a0e278075b638ae32db2f5ea8567d76a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine3.15`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-linux`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-linux` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-nanoserver`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-nanoserver-1809`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-scratch`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-scratch` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-windowsservercore`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1`

```console
$ docker pull nats@sha256:3ac4fc48a5f45ba948539c44528787c6a0e278075b638ae32db2f5ea8567d76a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7.1` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-alpine`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-alpine3.15`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.1-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-linux`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-nanoserver`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7.1-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-nanoserver-1809`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7.1-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-scratch`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-windowsservercore`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7.1-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2.7.1-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:dfe1a05929337ec7ed34a219272b33e2b6e4714026bda4d3f65ec76268c1d31e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:26978eb91b6f1aa3e255e1ed6c93cd09b25fd6ba284e8a9cd74bae36a3662ea3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf084274d588debf1c2d46247d20cb4f80d354aacb7604005572da5725c2a3fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:19:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:19:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:19:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:19:59 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:20:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fb380648df7ec4ba92f1d4d6ffdf641d6819466cce6509f667d94dad9f4c69`  
		Last Modified: Wed, 26 Jan 2022 01:20:55 GMT  
		Size: 4.8 MB (4752823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af65214d163d00ee68245e5e22e1265fec2c0c7f8e0ff23a89f90f9e4689a0`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55c8e4a874ee3840ec1c17b0f4143368c54e8fd6a755ffd09e1cdb8290815db`  
		Last Modified: Wed, 26 Jan 2022 01:20:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:b6a9f4ca613ad4869cb2048285f4bc14df63f5fda1926e40372cdb6958971766
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7050090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c9f21447079232e09b46ce60dc7bfc566b5cae47fe9d4100b4eabc6de14936b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:49:39 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:49:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:49:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:49:44 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:49:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:49:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2920b3e5877b294e547d8a1c4e3bd607d6d83ad295477663360ca72b6e5405`  
		Last Modified: Wed, 26 Jan 2022 00:51:54 GMT  
		Size: 4.4 MB (4417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fda4f318c0b4553cdc860867481a33a7dc2d3f2000375a6d2ee053a7f0bd6c`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8d7862ab8d965976774963f71fd952ad4c0d3a294fbd0034121f156e12327d`  
		Last Modified: Wed, 26 Jan 2022 00:51:51 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:219dd303cee8ae337143fe43e817e9ce1450302f257c28549de920aba7dcf73a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6845712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84db81365408c4dd9fc830a014f69e97973210f093c604deedf93de41f67a0b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 00:57:56 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 00:58:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 00:58:00 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 00:58:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 00:58:01 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 00:58:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6564f7bd948d1e195bd1386ecec2e370d1b2519e03c2063cc8789eb90c7ac1`  
		Last Modified: Wed, 26 Jan 2022 01:00:12 GMT  
		Size: 4.4 MB (4409947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30ca090f2ff1db96c07f94e0c463753271d0ef0e5b04768f02b4e5f737ec337`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74fc96dcbe074fbbffd72d2f6aecde13fbb3d4f5dbd99f56f69399990f575f`  
		Last Modified: Wed, 26 Jan 2022 01:00:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:daa50ac3732d7450e429c84a408abcc2940731eff3a98eac7d02fe8436fffe56
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7114110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422afb577fe2f6b912aa5793d6553b65bb59ae601e1fb3907b86db1dd09bc725`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 26 Jan 2022 01:55:21 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:55:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='44033b3e2652a6b56f10d8f7518e6152f026ec77f4937389c9e9b39c1fad664c' ;; 		armhf) natsArch='arm6'; sha256='e8e31f3c748c65ea475d9e83e04f62e381a87b7aeb8544945b3328d46ed2e798' ;; 		armv7) natsArch='arm7'; sha256='6445388443988a163b023ff3db8f539f0157fd400981969a383b6a4bf6519d4f' ;; 		x86_64) natsArch='amd64'; sha256='396e87f3b0f741d9190089766ca6c7fcf696c9282d730e5c1b62e34f84df673c' ;; 		x86) natsArch='386'; sha256='a354b576ad931a97a6ce5d248bd8013bb8a1077b3f195cf79bfd0069ba03d6a1' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 26 Jan 2022 01:55:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 26 Jan 2022 01:55:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 26 Jan 2022 01:55:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 01:55:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445060b32655cb4edfe06eac59815dabef07ff7dc77d6a7463d35b9b088aa395`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 4.4 MB (4397704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b12cd52fb778db44d89c0599ce5808fa58b7f70290c54a57a59c61eed5b92`  
		Last Modified: Wed, 26 Jan 2022 01:56:28 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1dc49cd213767a62d094faba237957b6f75ab6f11a040305af507228108cc7`  
		Last Modified: Wed, 26 Jan 2022 01:56:27 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:3ac4fc48a5f45ba948539c44528787c6a0e278075b638ae32db2f5ea8567d76a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:04eca2a64a16b320f79fab9bb3b11279b1833a919fe9d912d852856e2610cfa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:7a8486197e37bffe2a3dc83f47a56db1c73e8166a8132f42ea7b93e4870bb219
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718570368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24cd3e70e742b6d1b673b4d9dfb0e114b32fb8a1ef5ca8000d7d13f9b10e9aa8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Wed, 26 Jan 2022 01:15:09 GMT
ENV NATS_SERVER=2.7.1
# Wed, 26 Jan 2022 01:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.1/nats-server-v2.7.1-windows-amd64.zip
# Wed, 26 Jan 2022 01:15:12 GMT
ENV NATS_SERVER_SHASUM=0e7779836184c5b17c4c35e1cba992765fb85635ca8fea346ec86ec7ae4ff6cf
# Wed, 26 Jan 2022 01:16:33 GMT
RUN Set-PSDebug -Trace 2
# Wed, 26 Jan 2022 01:18:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 26 Jan 2022 01:18:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:23 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:24 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:25 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:130fffdf71021203b52a617e9f16e07be668fbca37bec3fad3eac2a97ec524f0`  
		Last Modified: Wed, 26 Jan 2022 01:19:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b504d7a94ab132597dcf74b8cbf17cc7a17e783f255872df856ea07c58a75788`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c6d127885f1d92e47e9c36b4ec6b24639dadc214c2f2ee065d1edbd8368f7`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9475de4454bc8233f08fb438730c876bd89ccba86bd4390c5e7112d464942ff`  
		Last Modified: Wed, 26 Jan 2022 01:19:14 GMT  
		Size: 369.0 KB (368968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e05dedf3be5135a21b615291e09e76255bcba11e302a8ece3a7db9f9ca09a4`  
		Last Modified: Wed, 26 Jan 2022 01:19:17 GMT  
		Size: 4.9 MB (4866549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7404ea55a5ea8d1ea0b8862a19889cda873685d749366eb82d4f5bf2af9d7514`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d508bca95ce19ff2406b565cac50a33b3d98d71b90035cab50b0f13900ed5`  
		Last Modified: Wed, 26 Jan 2022 01:19:13 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1667a90cbea2a31368941c21c1431c39385587571d8546e84085fdb86cac077c`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ae71e5f9694b1b41fffe7d12ff8be9c850e39fbd56d37f18e4ee99d5e4134b`  
		Last Modified: Wed, 26 Jan 2022 01:19:12 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
