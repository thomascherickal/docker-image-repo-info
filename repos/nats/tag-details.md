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
-	[`nats:2.6.4`](#nats264)
-	[`nats:2.6.4-alpine`](#nats264-alpine)
-	[`nats:2.6.4-alpine3.14`](#nats264-alpine314)
-	[`nats:2.6.4-linux`](#nats264-linux)
-	[`nats:2.6.4-nanoserver`](#nats264-nanoserver)
-	[`nats:2.6.4-nanoserver-1809`](#nats264-nanoserver-1809)
-	[`nats:2.6.4-scratch`](#nats264-scratch)
-	[`nats:2.6.4-windowsservercore`](#nats264-windowsservercore)
-	[`nats:2.6.4-windowsservercore-1809`](#nats264-windowsservercore-1809)
-	[`nats:2.6.4-windowsservercore-ltsc2016`](#nats264-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:2dbf782a59436baf0b71a6da774a3f4a641c085127f9aa4edbed3179eb008a96
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
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:3ebb22dda82aaa78924d827dc5508040067f75317cf53a045d5d7aeab0ac51be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:c68c9648e746aa0d68692c1bc2d5e84846ae287a78fb5b4c8d703f0a5dbbd325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:4217e9c0456e23c0270b647422b0b6c906d6e131c1ad91875b056f5715ac2bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6`

```console
$ docker pull nats@sha256:2dbf782a59436baf0b71a6da774a3f4a641c085127f9aa4edbed3179eb008a96
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
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine3.14`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-linux`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-scratch`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore`

```console
$ docker pull nats@sha256:3ebb22dda82aaa78924d827dc5508040067f75317cf53a045d5d7aeab0ac51be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:c68c9648e746aa0d68692c1bc2d5e84846ae287a78fb5b4c8d703f0a5dbbd325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:4217e9c0456e23c0270b647422b0b6c906d6e131c1ad91875b056f5715ac2bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4`

```console
$ docker pull nats@sha256:4c98fb00f39629814affa70733fb18a7b5683004d96f668e4bfaad70ef276690
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.4` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-alpine`

```console
$ docker pull nats@sha256:f1e53c6e766315c1554bcc7e45a59d6b3fbaffad6954e7f7e77fe5da0d922601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-alpine3.14`

```console
$ docker pull nats@sha256:f1e53c6e766315c1554bcc7e45a59d6b3fbaffad6954e7f7e77fe5da0d922601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.4-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-linux`

```console
$ docker pull nats@sha256:6ee1853e8914c5abf593af55dc67e6eb40d5961e190693ae6a50a00859aa3348
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-nanoserver`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.4-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-nanoserver-1809`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.4-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-scratch`

```console
$ docker pull nats@sha256:6ee1853e8914c5abf593af55dc67e6eb40d5961e190693ae6a50a00859aa3348
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.6.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-windowsservercore`

```console
$ docker pull nats@sha256:3ebb22dda82aaa78924d827dc5508040067f75317cf53a045d5d7aeab0ac51be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.4-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.4-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:c68c9648e746aa0d68692c1bc2d5e84846ae287a78fb5b4c8d703f0a5dbbd325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.4-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:4217e9c0456e23c0270b647422b0b6c906d6e131c1ad91875b056f5715ac2bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:ef3d1ae53d784bc4e2af8976b0747b9415ce02cdb600e9ca2c4cf77af3fe1263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:35de4fd5c9914ee78258e078bf8848c996e9808b71f98d3e5270c48a6876497e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7670678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015d08eea742029d6f2bc5f49d821d070e8de1c608977b6ad102c597172b9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:48 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:52 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dbd1b552429b94af686e909ab99c9ece98e65350d3cbf389432d62b2d7c090`  
		Last Modified: Fri, 05 Nov 2021 01:41:25 GMT  
		Size: 4.9 MB (4855262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7add72251f0d0b2329a59198077fb151a377e8b72aa23a8437b70dcb8540f419`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d0b4685a9c269b10e5ee30e79a48278a908bef37059e12b01a5665e4b22c03`  
		Last Modified: Fri, 05 Nov 2021 01:41:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:e9ff1076460bd51e94869672f4996e3ded4a7087a95cf767469df3677befaf52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7146549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84041734d375114ef2ec055c525298746ab688780fbf8e92b7896454c17dbe3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:40:33 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:40:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:40:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:40:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:40:40 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:40:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6efeedaac48bf3ed39c1ca63c1716f125f2c8a8de81c2e3ef12f6bdd2c306`  
		Last Modified: Fri, 05 Nov 2021 01:42:46 GMT  
		Size: 4.5 MB (4518134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5de06deee3394e8ce67d7707626d1feee02ccfa3f7aa8dec36479b14a2ba7e`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb681e323f9dcb73fbac5fa5b41efcd68e6c6561ab80d91c2cdffb06e8ab660`  
		Last Modified: Fri, 05 Nov 2021 01:42:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:47b0344f3d2f2786d736f4611d7af94e344ccf11d90e11de3872e48088a22ce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7179530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93e9fadff8a0152d6a077181ef0ebaf7dd47c0054f7e9a276794733ba015507d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 05 Nov 2021 01:25:08 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:25:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ff37771c0442e5921dd6867ef712c4029375a134f478b45469f5649b31ca06ae' ;; 		armhf) natsArch='arm6'; sha256='47b58410696fc2bbdd4b0c604f8a6df74b348bcf56efcff739a84f8c3da16f22' ;; 		armv7) natsArch='arm7'; sha256='071a52917aa7931dcce84d052e01310edd82d7399b5d699ddf9ad981af58fa5b' ;; 		x86_64) natsArch='amd64'; sha256='8a81d7c2c65f698875f5ed36cca842e37e51eb9bddb2374690d49bdc782aa6f5' ;; 		x86) natsArch='386'; sha256='659e085ed13d51acf52468e6e44257bf3dac3111ddf90ba065beb9a3c0a71b32' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 05 Nov 2021 01:25:13 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 05 Nov 2021 01:25:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 05 Nov 2021 01:25:14 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Nov 2021 01:25:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8711c96f805e6e7136f4ee5ebb812dd20a0dad59731799e120fd8515e4640d`  
		Last Modified: Fri, 05 Nov 2021 01:26:15 GMT  
		Size: 4.5 MB (4466763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b1eea8635159a074486029a3209c2391695c2693330521036c19b86572e8b1`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf26189c1b064d40e567961fcb53ae931fb2773f5c84be3be13e54495c5083e`  
		Last Modified: Fri, 05 Nov 2021 01:26:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:2dbf782a59436baf0b71a6da774a3f4a641c085127f9aa4edbed3179eb008a96
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
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
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
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:3ebb22dda82aaa78924d827dc5508040067f75317cf53a045d5d7aeab0ac51be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:c68c9648e746aa0d68692c1bc2d5e84846ae287a78fb5b4c8d703f0a5dbbd325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:99925ad515e56ad8aa6005447f289f1125aacc8791b34c22aeeaba585339cc1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691662407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f2030a37cdd58b62243e27c311718a0aa2e4eae5c55a51958d6ebcc649d158`
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
# Fri, 05 Nov 2021 01:14:03 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:14:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:14:05 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:15:02 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:25 GMT
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
	-	`sha256:92a7aa0a570a61f9cad71bac12d5309558ebfff4512f266a9c84d7fffe35567c`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0eeab78118391a7a40a7dcc21faeec0b8b70d97bc73513e824bf1b18af04ba0`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b581ca4c68730aff7d44f3932d39fc5e150ca9b86611ee88946d3286290bc88`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b25f9e002a677dfeb5a5858645aae7152cfd06648ec0355b74867f7b9bcfc4`  
		Last Modified: Fri, 05 Nov 2021 01:20:05 GMT  
		Size: 358.7 KB (358686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e7558373f528b98a0a139505b207c41c5936df7353547b07053164ef1dd481`  
		Last Modified: Fri, 05 Nov 2021 01:20:08 GMT  
		Size: 5.0 MB (4971837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eca02754ca6054523bd8d5140a6c126d7d1cee2051500a26fd0983ced3f67f`  
		Last Modified: Fri, 05 Nov 2021 01:20:02 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba6db01ad66aca0d878058c52c631b88fd6f61c826ef99d6a4d4b44ac3cf82`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191872413bf30200866dfee99486a08a953e72489cc3048908a39ee2ad394a0b`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6dbef5c6333e337297d86ba8533f288ea753e60925429ccf79365d2d865869`  
		Last Modified: Fri, 05 Nov 2021 01:20:03 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:4217e9c0456e23c0270b647422b0b6c906d6e131c1ad91875b056f5715ac2bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:b4fb2d1971400241bf4b12c3c275852080234036875786f6f3ec047c977a8d24
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278130219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09195455b6c7913f762585057b76bb9992818c08989744170f08f2ba2ce4d27d`
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
# Fri, 05 Nov 2021 01:16:55 GMT
ENV NATS_SERVER=2.6.4
# Fri, 05 Nov 2021 01:16:56 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.4/nats-server-v2.6.4-windows-amd64.zip
# Fri, 05 Nov 2021 01:16:57 GMT
ENV NATS_SERVER_SHASUM=e287764a6e8b8ec132dcbe294aa3b96d779678079b7ada20a9bde1b81d5f5bbc
# Fri, 05 Nov 2021 01:17:55 GMT
RUN Set-PSDebug -Trace 2
# Fri, 05 Nov 2021 01:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 05 Nov 2021 01:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:19:22 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:19:23 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:19:24 GMT
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
	-	`sha256:dc9668a0f5c066b47158130df6bdb6e41476ca682fbdab1abb5ef48f93b98c45`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c5f147d7adea9a440ba4690d881401198a8e6891535cd45b2c99093b985ea`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0de229c71c458655eecbd24455163aa6fa25b9b2a821136053044db0028e981`  
		Last Modified: Fri, 05 Nov 2021 01:20:40 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f615f95c20d2d9be2515be5e63923d4ebe1054f49ad986a1c8640fd9387d17`  
		Last Modified: Fri, 05 Nov 2021 01:20:39 GMT  
		Size: 348.4 KB (348419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22511f84b8f13d46f300e42b033581e0ca8a30ea44ba39aa6bab4d7fe2ebdc2`  
		Last Modified: Fri, 05 Nov 2021 01:20:38 GMT  
		Size: 5.0 MB (5002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b626a9695a8f3a79bf8c1a3f8d7241f8e6f954306a5068287b87e66e8a73e768`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 2.0 KB (1951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1476b22e04f3cf7c1ab8d1558bbbd9265ecefe83c819b6e8cd2a476a222ea16`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688d4de6a16e5e332914a38d5fd88e79174c2de65a20771aef43323a1ce802a3`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b9fec520215b911f107cda0b18f4fa69be800875aa730a76c4e2a57907c883`  
		Last Modified: Fri, 05 Nov 2021 01:20:37 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
