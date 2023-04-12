<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.17`](#nats2-alpine317)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.17`](#nats29-alpine317)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.15`](#nats2915)
-	[`nats:2.9.15-alpine`](#nats2915-alpine)
-	[`nats:2.9.15-alpine3.17`](#nats2915-alpine317)
-	[`nats:2.9.15-linux`](#nats2915-linux)
-	[`nats:2.9.15-nanoserver`](#nats2915-nanoserver)
-	[`nats:2.9.15-nanoserver-1809`](#nats2915-nanoserver-1809)
-	[`nats:2.9.15-scratch`](#nats2915-scratch)
-	[`nats:2.9.15-windowsservercore`](#nats2915-windowsservercore)
-	[`nats:2.9.15-windowsservercore-1809`](#nats2915-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.17`](#natsalpine317)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:190304122906415f1e9f343897d70f8c18d8c74b049c8de99af75081e453f76b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:190304122906415f1e9f343897d70f8c18d8c74b049c8de99af75081e453f76b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15`

```console
$ docker pull nats@sha256:190304122906415f1e9f343897d70f8c18d8c74b049c8de99af75081e453f76b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9.15` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-alpine`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-alpine` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-alpine3.17`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-linux`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-linux` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-nanoserver`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9.15-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-nanoserver-1809`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9.15-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-scratch`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-windowsservercore`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9.15-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-windowsservercore-1809`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:2.9.15-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:d26b2c764e207148f0f5d297bc003e5db69e59c0de197adb0a0254c3d84872e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:b8c33c1775880f98b37ec8555ccbb7ab2db2e89d807864dbce3abf18e0ee6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2be1dee271f717feb961aefbc00fbc062498bcfe2bfc68ef28f4993f4a0353c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:17:40 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 22:17:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 22:17:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 22:17:43 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 22:17:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:17:43 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b555478c97d500423b4ec4b759dea8d7222f5483c0d05faf690bcf65cca6b8b5`  
		Last Modified: Wed, 29 Mar 2023 22:18:00 GMT  
		Size: 5.3 MB (5260322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d097206350ad8a3fa170f350eaa1983c4aa285235aba3735eb54293cf68b1b5`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9acb3e08b26b83e42880e24fda19c80b1dc76010886c3e58a940e56d1a803fe`  
		Last Modified: Wed, 29 Mar 2023 22:17:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:a34069e01b53202550c58fb5ad62314ba3bd47bff825de7f9bf815e33db2e1d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187ff1764fbf00849fa72dd74711b2fc4604771b0810ec9d0f74b51dfa6e6a02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:25:56 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:25:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:25:59 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:25:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:25:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f6e895df39b31ddef480bd558704def131db5e52235a0f7f6d6a0e549ef48`  
		Last Modified: Wed, 29 Mar 2023 19:26:46 GMT  
		Size: 5.0 MB (5023853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185e76d48b40900624d64d497f45053dc1c8f1669fd5929d59fff490f1acd946`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907019fd32e315a992bdf93b69c2881d8583660aa015cd6f371aca1446ac7baa`  
		Last Modified: Wed, 29 Mar 2023 19:26:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:a07b10b9d4b0270547b1829ec2654e86f79abc88aacc6205185377e670505542
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79bb41326e49a9a4a84cd8fa0e6251ec300d8e66861fc5dedc6445c11b8d8bab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:24:01 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 19:24:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 19:24:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 19:24:04 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 19:24:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:24:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c782d9234ff70b39bfff1c9fae811b6502cb9f751cc42adb8fea7a1cae072b`  
		Last Modified: Wed, 29 Mar 2023 19:24:46 GMT  
		Size: 5.0 MB (5018067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6550b200cd2b3bc8c94ad0423e19eb7bb2111322df8eed66c3312d2d62b36ec3`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac38931f834e11c161f4de58f07336f18185b088a6306d3f9d3938945e360df`  
		Last Modified: Wed, 29 Mar 2023 19:24:45 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:26c93c2e512a5be5cf69f6a77981f65bd2a34aa0a267808a78044900523a2273
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8103920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6594aa95a6a12292c371fbbdb19b57c50f425b9f714408537241356a8489758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:28:21 GMT
ENV NATS_SERVER=2.9.15
# Wed, 29 Mar 2023 18:28:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 29 Mar 2023 18:28:23 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 29 Mar 2023 18:28:23 GMT
EXPOSE 4222 6222 8222
# Wed, 29 Mar 2023 18:28:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:28:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a70aa6cf97869cec2d16b8b65f99275cce8c3cf655624bfc181c7276d19641`  
		Last Modified: Wed, 29 Mar 2023 18:28:38 GMT  
		Size: 4.8 MB (4841068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a9ab842bf93fd56404bc8c33ba71ee9e747c755a2dc2c1720aa82c6b178aae`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52624160d291d3643a842fdeb0ad2337c0dded7d37ad0a250d2ec6ae7615b66`  
		Last Modified: Wed, 29 Mar 2023 18:28:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:190304122906415f1e9f343897d70f8c18d8c74b049c8de99af75081e453f76b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4252; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:1716e8fedea9b15759385f82c7c80d974a7a801afc4c2c28e1c21447f07f1f50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:6da565ba8ca15a6dc08ffbd4e747a6294c91028a817a24a64c0239a05e0739b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111822373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9692c57846a300005371142982859691fe3fee6be22d0eca5f9db333db43d5f4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Wed, 12 Apr 2023 02:46:54 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:46:56 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Wed, 12 Apr 2023 02:46:57 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:47:05 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:47:10 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc7d128fe5c7171551f4a377b11c36a7622d87a3d7acc003e8144ead046dbf`  
		Last Modified: Wed, 12 Apr 2023 02:48:07 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529b16ff56ca8331d0c5efa7e08607431529929fcc608f0b71fde3cc0ebf512`  
		Last Modified: Wed, 12 Apr 2023 02:48:06 GMT  
		Size: 5.0 MB (5026941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fa3ecf95c9443cbf2fd478990fc8bc4d937903cd4b5d28a27867d7329ae1a2`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c47224eef33521f5a81e38be5194f729f89642ce2d0522dcc22c30ae4d2e9`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98dc4124dae3afb1e28f55853747172c32bca24b1ca3cd288afeb4ad9acf4b7`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f68df75bfb7cbd69ac2bcafe08f7274f82533af2e02dffd14bebcb1009ffea`  
		Last Modified: Wed, 12 Apr 2023 02:48:04 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:e9767cfa85287292db74b0533d910366598f93e18b3c60706cf1c25ab7f657be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:1a82b1b261d169994fc6162f2f25894a49e20971560f8b2dff4f90eefb32b421
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4973038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74665a2673c052e85d3417cec864d1aabab3263f3328051037a133d9b85765ce`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:32a9f093b76345e99bd81ff00eabc5ab1ae6c2bdc7d6c843c923049ea3c620ce in /nats-server 
# Thu, 02 Mar 2023 19:20:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 19:20:01 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:20:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 19:20:01 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 19:20:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:436f213323b997ad7aca1675cce2c9a9366e3cd51995b9829835ab9762901f98`  
		Last Modified: Thu, 02 Mar 2023 19:20:48 GMT  
		Size: 5.0 MB (4972530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb98c93488e5f33bab9a8b331c5fbe988a9dd644e39cc15e6626550ec05e541`  
		Last Modified: Thu, 02 Mar 2023 19:20:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e1ba487c56a25895759177de201768f40c51ceeedca983afa03875039445bb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4739851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b60b5d45617b9109e120de34ac32b0647324dba3d69d2c56366545e50c2484c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:614e1182091dacdaa5043752e8239600bae8aa334cfd383cc326d1753d3eba64 in /nats-server 
# Thu, 02 Mar 2023 18:49:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:49:36 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:49:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:49:36 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:49:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d859c106d4072b51eee7be282394c7f0c288186311ae904751cd95c3cf9468ae`  
		Last Modified: Thu, 02 Mar 2023 18:50:54 GMT  
		Size: 4.7 MB (4739343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e7000b41bf11d721897d126c1e72201203bcc8e9716daad77d7d42ae97853a`  
		Last Modified: Thu, 02 Mar 2023 18:50:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:644eac35d964521bc85286defaf1bae093b36618fe862eedff9a996e330fc60c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4731109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e814afeda8d92b2fb3dcdacf4648234504c6e4cd7fc24cce256cc588a439d7e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:a63786ae76c5e718a4952dd30b2265019e1ca48099ad19279d2e77e5ad704bfc in /nats-server 
# Thu, 02 Mar 2023 18:57:49 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:57:50 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:57:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:57:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e714c80855fb90cb44f135a04bf323493a749536bb9106eb3ef4e69a70682897`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 4.7 MB (4730600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e020ba411c44ee7d23b6bdbd966700955c2d087afd3d79a9ad51e0390e8e7b6`  
		Last Modified: Thu, 02 Mar 2023 18:59:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:35ef84ac5e9bb0d0229fb1a773677d6ee7b23bb58937427d20aaa36987562373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4559479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f367536d7ef4331c52bf405914c6f7affdccdb8eed05fb4c981efe519fd06f00`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:23081283f9b4d8145ad2b3a276cc08fcb49c4850e322db9560525e495d1bf362 in /nats-server 
# Thu, 02 Mar 2023 18:40:16 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Mar 2023 18:40:16 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:40:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Mar 2023 18:40:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Mar 2023 18:40:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a910efaa632bb8401dbca7cfe541f6dc4da71ea38708992ef153250254493114`  
		Last Modified: Thu, 02 Mar 2023 18:41:09 GMT  
		Size: 4.6 MB (4558972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be7fc9abf13897cf1a5e7026f6a49b3308d5a864640e1f4b6e526ee95f093fc`  
		Last Modified: Thu, 02 Mar 2023 18:41:08 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:e7f84cdd956a876ab908cdd0f219a594983dad87d2260f0b55254ac2b6053840
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull nats@sha256:a520b56fd1c9b6ca9c16ea84c31de7397f27906b003b77321f2a1f92e9bf989d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077192970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5096d5c9d43d0360e18472178afc4325d69b0d268b74eec1d604705b001d7d4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Wed, 12 Apr 2023 00:18:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Apr 2023 02:41:25 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 Apr 2023 02:41:26 GMT
ENV NATS_SERVER=2.9.15
# Wed, 12 Apr 2023 02:41:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Wed, 12 Apr 2023 02:41:28 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Wed, 12 Apr 2023 02:43:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 Apr 2023 02:46:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 Apr 2023 02:46:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 12 Apr 2023 02:46:20 GMT
EXPOSE 4222 6222 8222
# Wed, 12 Apr 2023 02:46:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 Apr 2023 02:46:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81203863a516fb636d8e06e71cc938e6621b372bd98921ce87d23012f6c9e4c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e5d770cd81ae0b8d0e969f23155d2900d6270b1dd31877d3d940112d6c37c`  
		Last Modified: Wed, 12 Apr 2023 02:47:45 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d654aed9de676c8c15b484ab00ae4844ba79daf4719575483ac1713c1fea79e5`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6971dd6b86955eb21ff8ff2fc06867f884a06195e44d97db038e01149045ce7f`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1547986644868ba699177eec8a522abf35d0b1eeca5b66a23c5250d6e683`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4079076d2a3e2cd7f12825a33036fbc3e18a4cad17a79cb53bc17f9e443891`  
		Last Modified: Wed, 12 Apr 2023 02:47:43 GMT  
		Size: 495.6 KB (495591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1aa8f2c9e3b66af0ee150f08b553ccd38d2baeaa402a72b5105a707903d6cfd`  
		Last Modified: Wed, 12 Apr 2023 02:47:42 GMT  
		Size: 5.4 MB (5392873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608c53cc0c946ad500fdbdd81bf5f958f50b2105245342976714ebc075160b9`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 2.0 KB (2023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ae2de115b72a4c93eeba7e35bc9dae9ccedb47373b06587d415d0458d242f`  
		Last Modified: Wed, 12 Apr 2023 02:47:41 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fea7926103053f3ba1668e1ba8cc86fe5e6f2442f53e36d435401c3a9cb094f`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ca86945cd5e9cadc7e0297ae741b3ee5d5f1093d44e9f9a0165755ce4b362a`  
		Last Modified: Wed, 12 Apr 2023 02:47:40 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
