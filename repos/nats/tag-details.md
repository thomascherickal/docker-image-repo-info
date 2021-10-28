<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.14`](#nats2-alpine314)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.6`](#nats26)
-	[`nats:2.6-alpine`](#nats26-alpine)
-	[`nats:2.6-alpine3.14`](#nats26-alpine314)
-	[`nats:2.6-linux`](#nats26-linux)
-	[`nats:2.6-nanoserver`](#nats26-nanoserver)
-	[`nats:2.6-nanoserver-1809`](#nats26-nanoserver-1809)
-	[`nats:2.6-scratch`](#nats26-scratch)
-	[`nats:2.6-windowsservercore`](#nats26-windowsservercore)
-	[`nats:2.6-windowsservercore-1809`](#nats26-windowsservercore-1809)
-	[`nats:2.6-windowsservercore-ltsc2016`](#nats26-windowsservercore-ltsc2016)
-	[`nats:2.6.3`](#nats263)
-	[`nats:2.6.3-alpine`](#nats263-alpine)
-	[`nats:2.6.3-alpine3.14`](#nats263-alpine314)
-	[`nats:2.6.3-linux`](#nats263-linux)
-	[`nats:2.6.3-nanoserver`](#nats263-nanoserver)
-	[`nats:2.6.3-nanoserver-1809`](#nats263-nanoserver-1809)
-	[`nats:2.6.3-scratch`](#nats263-scratch)
-	[`nats:2.6.3-windowsservercore`](#nats263-windowsservercore)
-	[`nats:2.6.3-windowsservercore-1809`](#nats263-windowsservercore-1809)
-	[`nats:2.6.3-windowsservercore-ltsc2016`](#nats263-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.14`](#natsalpine314)
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
$ docker pull nats@sha256:5e6c045053b9de5271f6a55973ee34a16310eb1fada9ccc013f3d78fb06ed643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f800e2895004eb8f215d1a19eda82f1d0680915ad0111eab250fdc5bc0d375bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a368c33c6a0eb0e674c90b2fe891a4f381e666b015dc6f690dc143a2c0f54d3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:66e5dfec5b380717e7d72eb0559430d619858fb7e561bf035f4e05d29bd2f30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6`

```console
$ docker pull nats@sha256:5e6c045053b9de5271f6a55973ee34a16310eb1fada9ccc013f3d78fb06ed643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine3.14`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-linux`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-scratch`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore`

```console
$ docker pull nats@sha256:f800e2895004eb8f215d1a19eda82f1d0680915ad0111eab250fdc5bc0d375bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:a368c33c6a0eb0e674c90b2fe891a4f381e666b015dc6f690dc143a2c0f54d3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:66e5dfec5b380717e7d72eb0559430d619858fb7e561bf035f4e05d29bd2f30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3`

```console
$ docker pull nats@sha256:54846966574ad3a6b2e8efe1e6dfa1972fccfe1a2f90f813898d725bdbc2ca99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.3` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-alpine`

```console
$ docker pull nats@sha256:218be65ec9065f8087b664ae7204602c12d2e974b973913b9099356710002c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-alpine3.14`

```console
$ docker pull nats@sha256:218be65ec9065f8087b664ae7204602c12d2e974b973913b9099356710002c08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.3-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-linux`

```console
$ docker pull nats@sha256:90eb587919289d4bedc3ceaf8fea4719913fafba831302548cb2840d9a615641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-nanoserver`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.3-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-nanoserver-1809`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.3-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-scratch`

```console
$ docker pull nats@sha256:90eb587919289d4bedc3ceaf8fea4719913fafba831302548cb2840d9a615641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-windowsservercore`

```console
$ docker pull nats@sha256:f800e2895004eb8f215d1a19eda82f1d0680915ad0111eab250fdc5bc0d375bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.3-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.3-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:a368c33c6a0eb0e674c90b2fe891a4f381e666b015dc6f690dc143a2c0f54d3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.3-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:66e5dfec5b380717e7d72eb0559430d619858fb7e561bf035f4e05d29bd2f30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:a76e3b6f5099cb61bca36a882adb5f6e68f3d64a3d328f082f7df5d075ab422b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:3635753f0dcf4d6221fc95ce5498417e90229e779e6121ee7c28d24aeab80708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6936463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774d308723b8e05215d6770933bbd689cdc7fd5475e1cb71247a7569d4b8e4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 09:02:21 GMT
ENV NATS_SERVER=2.6.2
# Thu, 14 Oct 2021 09:02:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 14 Oct 2021 09:02:27 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 14 Oct 2021 09:02:28 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Oct 2021 09:02:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60d9422376f2fa0c35dc1093259c916a4eb0be4a60a4d9a961fe0996c66ab4`  
		Last Modified: Thu, 14 Oct 2021 09:04:45 GMT  
		Size: 4.5 MB (4505071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83b74f9c459e2fdba66774799e4ff8a27253139d4cacb60a5fcd9694c63250`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8104368edaad4864ffa5ae52d9a7eab3276b91767d671069ebdac1a0cbbbd`  
		Last Modified: Thu, 14 Oct 2021 09:04:43 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:5e6c045053b9de5271f6a55973ee34a16310eb1fada9ccc013f3d78fb06ed643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:c3ae79082e1f6e41c15eead75a1cb23853959f99d930bcde514992b68614b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f8c670702f9c985e69da5e7fd47faad2916a7fc779813cd5750ea0229d81d667
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4221946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afffea752a48540e5d479625fb0d6e9741dc2bafcd8ac41276ea1b204453a235`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:9a54a4b91cc53aa015be15163985c3a1e9f5b65cc100b3881622a2ec707ec7ed in /nats-server 
# Thu, 14 Oct 2021 09:02:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 14 Oct 2021 09:02:58 GMT
EXPOSE 4222 6222 8222
# Thu, 14 Oct 2021 09:02:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 14 Oct 2021 09:02:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12aa08ce2b8ebed90e814474b61290a6d2e1656de5f6b64c0cfa4208b17e823b`  
		Last Modified: Thu, 14 Oct 2021 09:05:24 GMT  
		Size: 4.2 MB (4221469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017cd1d70fd1ded785cbf5e165b2d1752afaf1fcae97d07ea7a75abba99516c`  
		Last Modified: Thu, 14 Oct 2021 09:05:21 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:f800e2895004eb8f215d1a19eda82f1d0680915ad0111eab250fdc5bc0d375bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a368c33c6a0eb0e674c90b2fe891a4f381e666b015dc6f690dc143a2c0f54d3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:51a7ac5e0fd77e0d518cacc4ba8dd1ef7247cbeb90d2efc2aa36a8e2e8a18e4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691656157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:094b345fd0b9938b0e78ff8e1a41bd7a948a5d96fd0e5614e7dc9f4c4c105b0c`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:14:51 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:14:52 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:14:53 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:15:57 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:17:23 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:17:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:24 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:26 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:d5c6b53d16e827fcca445a1d26aa91959d444f28e2137fe5fbfcf6f0e8fc54c7`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00da00af251dabde3e8ca9fac5e98e48957058ae66cfc6cd227cf53306475289`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3723fb43a09376bf4c64c3a7bda1347b72d6b6d4b1c154e18966fbe654d672`  
		Last Modified: Thu, 28 Oct 2021 22:20:58 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c450ca9bbda8ce4628f97b0e1ad60d3a60e9ea834594497f45d4ba31906dccae`  
		Last Modified: Thu, 28 Oct 2021 22:20:57 GMT  
		Size: 358.7 KB (358737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef148399e4f9c2b7d805a4f81063d19e5d1f0af2e7cf825c953d6485930ba268`  
		Last Modified: Thu, 28 Oct 2021 22:20:56 GMT  
		Size: 5.0 MB (4965585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e2a9be13aa047556c95aa527fb1309844e9c568b6f7d47b512cc82e9898064`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.9 KB (1924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b1f93d27be52abceae707d37a2208c1754ef97d1df70376d2231249e719d2c`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980a908f4dc78616da8546ec4997c9b27ee6e032da4f9315fad2bf9965451458`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111fccb3f1e5ffbda9b83e6a4b670382b282db49b4d6cd7a30631b7a7de6c82e`  
		Last Modified: Thu, 28 Oct 2021 22:20:55 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:66e5dfec5b380717e7d72eb0559430d619858fb7e561bf035f4e05d29bd2f30f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:7e87d39f63d888a8c38989beda927f43d801c6fc88dbc230a2b8b600afd2b569
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278116707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1342ba4bbfda650dd7a22cc73f3eafe211dbcdf3d88c445b13b5e1e3ed24dec6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
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
# Thu, 28 Oct 2021 22:17:45 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:17:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.3/nats-server-v2.6.3-windows-amd64.zip
# Thu, 28 Oct 2021 22:17:47 GMT
ENV NATS_SERVER_SHASUM=f06c5434d375016946993ad3c505c8e7b391b0dfce8afdc82d83ab43c74d155e
# Thu, 28 Oct 2021 22:18:48 GMT
RUN Set-PSDebug -Trace 2
# Thu, 28 Oct 2021 22:20:18 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 28 Oct 2021 22:20:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:20:20 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:20:21 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:20:21 GMT
CMD ["--config" "nats-server.conf"]
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
	-	`sha256:4b125ecbbd9fcd1e607a95ad95618b22bed487633e2c3f53e74079496cbf3e7d`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d36335126bc1a01fd80e6e62c8b12b80a4ba0930c9044553d759ed416c9ad5a`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6861aaad346207f6efc3d74dce720f56b81d8292a8f10b16a126d3545a67c784`  
		Last Modified: Thu, 28 Oct 2021 22:21:29 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee10f08ed053b70ed8c754e81edf0e43eb621718ec915d979bc4515f6bf3614`  
		Last Modified: Thu, 28 Oct 2021 22:21:30 GMT  
		Size: 347.5 KB (347462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72024e6801dae28939f9b887af08469d17db75599cdace64ba5ad1bc46105392`  
		Last Modified: Thu, 28 Oct 2021 22:21:33 GMT  
		Size: 5.0 MB (4989467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e989943b45c1112cb4df4c4b061238abebaf0125af3515e0cec1837b2bd21d`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 2.0 KB (1977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811eabaa8cb45eb635eb3de73e9905648c98a5aaace1cfc8af9019f280ce424`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08391a88082294bf9684ce0626a570685c8056c6e61e3f73e6763d4870ad05`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7666d9a660e321d771c0067346cb4c5e6807397c8be963e1c7461161d0f0e6ad`  
		Last Modified: Thu, 28 Oct 2021 22:21:27 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
