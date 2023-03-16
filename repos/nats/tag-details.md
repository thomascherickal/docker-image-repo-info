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
$ docker pull nats@sha256:58e483681983f87fdc738e980d582d4cc7218914c4f0056d36bab0c5acfc5a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4131; amd64

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

### `nats:2` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:58e483681983f87fdc738e980d582d4cc7218914c4f0056d36bab0c5acfc5a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4131; amd64

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

### `nats:2.9` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15`

```console
$ docker pull nats@sha256:58e483681983f87fdc738e980d582d4cc7218914c4f0056d36bab0c5acfc5a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4131; amd64

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

### `nats:2.9.15` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-alpine`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-alpine` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-alpine3.17`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.15-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.15-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9.15-nanoserver` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-nanoserver-1809`

```console
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9.15-nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9.15-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.15-windowsservercore-1809`

```console
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:2.9.15-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:0158c030a6be61a98a76e10101dc3f48fa328b362806d18930162e7a1ac2c6a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:9947eac2dedc476378d9cac73c7df6cba2f1a23da12137214cdc254a15863a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8635785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90d6b3fd56dc8fe20a6e41de4afeacff348a53e1ab388f535f404e9cf74c084d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 19:19:49 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 19:19:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 19:19:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 19:19:52 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 19:19:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 19:19:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08472afe1eaab0ac7a92349d2da3b64cafacc125426338b278e2fc3b006bd52`  
		Last Modified: Thu, 02 Mar 2023 19:20:25 GMT  
		Size: 5.3 MB (5260338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5ae32cc4383cc8cabea2eba8667d1ff1aaa9bf699469141395387df31c5c4b`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f805284c458c477cde0410e2f6835ab92c5fd6b464cfd6c07cf3d52643c23`  
		Last Modified: Thu, 02 Mar 2023 19:20:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:2003c1a533556804861ebff12c6f6baeb1fb16e7f454efbe05f659dea1c220b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8135735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baaac2464d927841294d5f4482db763fe11d3a345db922c3be854b1148252fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:42:08 GMT
ENV NATS_SERVER=2.9.15
# Tue, 14 Mar 2023 01:42:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 14 Mar 2023 01:42:11 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 14 Mar 2023 01:42:11 GMT
EXPOSE 4222 6222 8222
# Tue, 14 Mar 2023 01:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 01:42:11 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918accfe9dcdaeba9c46ce13661f9dfbf5489c196b0f61b91191b9ed665aad7`  
		Last Modified: Tue, 14 Mar 2023 01:43:02 GMT  
		Size: 5.0 MB (5023852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cb1a87eed59db0bae3597c0c889575ed3c76db4192c528553f6c8d54be638c`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2960cc2a0c59d3d72339a68f259594245f538daf938f276b1a716b851d3c1`  
		Last Modified: Tue, 14 Mar 2023 01:43:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:4d0f535bd276e1b92c60c9b8fe33cb90d439049071159843142c026302b54bf7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7887576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b405c7e2612cb810f225540c61a3eb1f02c1efbb3910aa30aa7b46b068fef2db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:57:36 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:57:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:57:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:57:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:57:39 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:57:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b56339a1ba27c396a17554216f8da9ef664a78ec52c24c39630ad6b00ccea`  
		Last Modified: Thu, 02 Mar 2023 18:58:37 GMT  
		Size: 5.0 MB (5018081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6919af5eaed170352d5fcbc4a52cdfd188a277c02b8c39538f0626a12afc6e`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99bb0ebd369abc6e32fcdbdbade73f2a1504cb8edae42327051d1343b982a8b`  
		Last Modified: Thu, 02 Mar 2023 18:58:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:31516678d6c3c1c5d7444e85d06618022258cfb3a23bbed0e44a358bbf7fea1a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8104002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39f18af0a035256392dde53a51a48628b107ebad3b4b6627160aaab7a964ce40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 18:39:45 GMT
ENV NATS_SERVER=2.9.15
# Thu, 02 Mar 2023 18:39:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f4f86a5c10914bc6fb40effd2fdaa3d4f69bbbd14ca68571c4afe49c7cd1356d' ;; 		armhf) natsArch='arm6'; sha256='29c8e26624011d05a2befcb3a25d00eaae098baba34f02e93cc3e336b6aa61ec' ;; 		armv7) natsArch='arm7'; sha256='83b6c1cb1b9d7d15b6fa042b63bd4af1cd66884d1b46849ba362b171611c19ad' ;; 		x86_64) natsArch='amd64'; sha256='32ba26c522b3c245f2105e9642256b0bd8f993f3f9a034b701a327721576d761' ;; 		x86) natsArch='386'; sha256='b32b54780fdc7527e0414a852effbbfab8e2c3f3482935b9459f586095e39945' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 02 Mar 2023 18:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 02 Mar 2023 18:39:47 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Mar 2023 18:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 18:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f03396fa041b5be75e5a939ff3aadaff2e65f529a07bcbd4748b581e3e193e1`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 4.8 MB (4841045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cceddcd111b1a86e5348af7dccf8c0b0d1c1dfec305c026bd9351bd0d1cce7`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca183fb542756060f50207e2bdac939b035a4f4ff2075b0371f87399242950a2`  
		Last Modified: Thu, 02 Mar 2023 18:40:46 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:58e483681983f87fdc738e980d582d4cc7218914c4f0056d36bab0c5acfc5a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4131; amd64

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

### `nats:latest` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:nanoserver` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:e37929e6e16e54eea197ddd116aab3e276eff98032095765851fb52f7a05dc4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:cb3ba37461683f06b1d00ad0bb4dcaddcc31331140451fe23c60bbc3984aa383
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111717590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9436691874ee5383809fce5c0233247c872f3646c4b5706f22aa4219053bbbbb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 04:09:13 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:13:02 GMT
RUN cmd /S /C #(nop) COPY file:c0761502e8e3e74fa63209f49b4d4f61a9c596c726f61d96e045d0b22538ada5 in C:\nats-server.exe 
# Thu, 16 Mar 2023 04:13:03 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:13:04 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:13:05 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989bf40c40575727f8231d233b462fde8f135997008e29030565a868625bf08e`  
		Last Modified: Thu, 16 Mar 2023 09:07:41 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16a55dca6f08e1b0f6ab504240dcbefa2967791e859291f91cf2975c5c2dc71`  
		Last Modified: Thu, 16 Mar 2023 09:07:40 GMT  
		Size: 5.0 MB (5026906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cea4f67910effcd674e1af18718629fecd35ba5766bbd51b0c873e7dad418a`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b128e2fbc1ad408e14ed993144bd9f274db73e7d5e78ea48571e0c7ecc95cf54`  
		Last Modified: Thu, 16 Mar 2023 09:07:39 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2345dd4b412c374fb3c37671d6b57f967dfd1c3d03af8298cbd354108c4eab1`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc1f4027df8fb816a73fa0b8839a628e8b3188415f2f934e9c3dca7ad65cea8`  
		Last Modified: Thu, 16 Mar 2023 09:07:38 GMT  
		Size: 1.2 KB (1170 bytes)  
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
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f5022549bc80a9db2612765446cab1bfd7a1be26e723a61158bc4b0c031f5fec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull nats@sha256:836eedb3e349b1f2b43a2a8a1075a7c75daec9d12da9a688fbf0e0ccc6f5f900
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2019348725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4cd0dd10b5e08978a6e679dbfbbc002970ff7ae24add62a49afe725523436b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 02:59:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Mar 2023 04:05:12 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Mar 2023 04:09:46 GMT
ENV NATS_SERVER=2.9.15
# Thu, 16 Mar 2023 04:09:47 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.15/nats-server-v2.9.15-windows-amd64.zip
# Thu, 16 Mar 2023 04:09:48 GMT
ENV NATS_SERVER_SHASUM=090f5c310beeb94f603898c6940f2793c292b20c131e578967fc2cdbd01bd42a
# Thu, 16 Mar 2023 04:10:58 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Mar 2023 04:12:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Mar 2023 04:12:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Mar 2023 04:12:51 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Mar 2023 04:12:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Mar 2023 04:12:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474eedda733dad347e4baad9fb9f3d700b58e5788f7453d1979cebb167746b32`  
		Last Modified: Thu, 16 Mar 2023 03:44:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c46bc18b88e816c6caaf34206ccb18a5b7f6665a73ae9a4678525d49fcb1f2`  
		Last Modified: Thu, 16 Mar 2023 09:07:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4a68e4291e27c96744fec7ab4710e923e5b1e40c9f3c6a2e92b8739a3d31b5`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459f257cce40d5f7ebac46302e2139fb4d25193d8d5cfead8e487c752e1b2d3`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6975473a2f80a1aefa9af46e42f89a933991476f79d5e5a2da8e146697cffe44`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22253a34963956a4b34689b662e68bd6064ddf0b8aed7177c361264681e439`  
		Last Modified: Thu, 16 Mar 2023 09:07:25 GMT  
		Size: 474.3 KB (474294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec188877326c722f291ad8e0486acf0351224348d1a7d5d69d2f46dd2b34d6b`  
		Last Modified: Thu, 16 Mar 2023 09:07:24 GMT  
		Size: 5.4 MB (5352102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaf0234efde44a2b0e27f3aad8cc98edda5e6d51bdfc76348701cfdbd1b4182`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6235fe1716486135953312ee3d91de53d571a34c36eb3af9ab08e7457ea13a3`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2ba63ea546de8e882e02776ea30e2b71555c06d83d435809a377b1e02a664f`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252cfddbc298f640d6da169c875464a1fe1c426dbe0c2564f3bbf7ddbc3cee8a`  
		Last Modified: Thu, 16 Mar 2023 09:07:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
