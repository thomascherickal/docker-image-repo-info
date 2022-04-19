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
-	[`nats:2.8`](#nats28)
-	[`nats:2.8-alpine`](#nats28-alpine)
-	[`nats:2.8-alpine3.15`](#nats28-alpine315)
-	[`nats:2.8-linux`](#nats28-linux)
-	[`nats:2.8-nanoserver`](#nats28-nanoserver)
-	[`nats:2.8-nanoserver-1809`](#nats28-nanoserver-1809)
-	[`nats:2.8-scratch`](#nats28-scratch)
-	[`nats:2.8-windowsservercore`](#nats28-windowsservercore)
-	[`nats:2.8-windowsservercore-1809`](#nats28-windowsservercore-1809)
-	[`nats:2.8.0`](#nats280)
-	[`nats:2.8.0-alpine`](#nats280-alpine)
-	[`nats:2.8.0-alpine3.15`](#nats280-alpine315)
-	[`nats:2.8.0-linux`](#nats280-linux)
-	[`nats:2.8.0-nanoserver`](#nats280-nanoserver)
-	[`nats:2.8.0-nanoserver-1809`](#nats280-nanoserver-1809)
-	[`nats:2.8.0-scratch`](#nats280-scratch)
-	[`nats:2.8.0-windowsservercore`](#nats280-windowsservercore)
-	[`nats:2.8.0-windowsservercore-1809`](#nats280-windowsservercore-1809)
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
$ docker pull nats@sha256:cd6b7fa512b8aa3115d3fb3980d3b3c025ece3afb163c33ca8f885cb9ca4a959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

```console
$ docker pull nats@sha256:cd6b7fa512b8aa3115d3fb3980d3b3c025ece3afb163c33ca8f885cb9ca4a959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine3.15`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-linux`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver-1809`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-scratch`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0`

```console
$ docker pull nats@sha256:cd6b7fa512b8aa3115d3fb3980d3b3c025ece3afb163c33ca8f885cb9ca4a959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.0` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-alpine`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.0-alpine` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-alpine3.15`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.0-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-linux`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.0-linux` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-nanoserver`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.0-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-nanoserver-1809`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.0-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-scratch`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.0-scratch` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-windowsservercore`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.0-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2.8.0-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:cd6b7fa512b8aa3115d3fb3980d3b3c025ece3afb163c33ca8f885cb9ca4a959
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2803; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:5ee908f70b2d8bae4fd68220285e7cbb50ac007bf664f3a49dfdf6eb92830bde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:bcd3a52a97e42d20d635f248df18ce26b32f33408239d1d92f993ee540d92957
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107723822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f7bc390ca6545a7c4a6258a183ea122410c6d26944dc65517bfa7fb7cf9f1ec`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:26:42 GMT
RUN cmd /S /C #(nop) COPY file:e7990ea3e8b3452cef0498934f2ec2cc0ec6064b6c561d6b6b0950f323493695 in C:\nats-server.exe 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:43 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:44 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:45 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a6063f744e542c21ce471bdd7ff0dd6063d8d2a9670afbbc64d086813afd6385`  
		Last Modified: Wed, 13 Apr 2022 14:46:35 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3dfac9c4e6275270f4294805bc3e9e32b7e2adc14a6f7bc5809e8c2f37b20f`  
		Last Modified: Tue, 19 Apr 2022 01:27:31 GMT  
		Size: 4.6 MB (4621267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7f8d6d038180903a45af2e6a737db2d6723199ae9b6a44a82f379cebf6e7e`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b50817233fdb21cd680ce186501ff45c6ba75a15430cf283b3a3cf18303a86`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d393a6134f8cf675b5eb18d3aa45a6d3a5bb0f144212b152a5a3bef7555f73`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87ab7743d2e9d63ba7893605c2c83f63d29579cef3b07ffb8d17dc765915139`  
		Last Modified: Tue, 19 Apr 2022 01:27:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:192e92df7beb0dc71a914ae8586d30817005435ef9567c7e47693ad170e28ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:8bd17688b3f48c3adfdab56d3effce03a361b1b47504f2e1e7350d59cd9daab2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4577760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d46ec68770eafbc93e836c7ec9872d55f6bfd6fb2af492abe4534b795547f6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:ca37028b27d839d950bcae33931d7e6615fb1b09323703fcf9eaa9647f444002 in /nats-server 
# Tue, 19 Apr 2022 03:06:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:06:10 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:06:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:06:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e9fc57d876d27155804078e28290d22cbba732762320a4daca2d681be9d5ac56`  
		Last Modified: Tue, 19 Apr 2022 03:06:58 GMT  
		Size: 4.6 MB (4577253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953499f4b34cabe7f9d88476ba63999880bf8aff1c88038d2fc6eb9c1c846b13`  
		Last Modified: Tue, 19 Apr 2022 03:06:57 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f1d583764567c881a0e61a2f17281162dd765f00db2474de4081a2b643e3d4c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af0f20fc23cdefbee46926169caa559e7a84f9204347b6426f377b91c9b69f27`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 01:55:37 GMT
COPY file:8cee33100ded62c397ffde3de5e9ea249d650168c802e2611fea578c07655f04 in /nats-server 
# Tue, 19 Apr 2022 01:55:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 01:55:38 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 01:55:39 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 01:55:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d693eff09d55c2616a7901f894d0d0f2498f5f28e23f3a863919e02e22a6ad`  
		Last Modified: Tue, 19 Apr 2022 01:57:59 GMT  
		Size: 4.2 MB (4236107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b54f80cb9d96012058f10a179ecd81de8d5505556b318b2400d3294ba4a9e9`  
		Last Modified: Tue, 19 Apr 2022 01:57:57 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3c8ce819721153ec2da8805ad16a87b94081820a66038d13707555ff80b1ca13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4230403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c2c0a899028f7cf702974f52380f0741fc608d28ab732b8d24fc5d20699dfae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 05:27:08 GMT
COPY file:5c7701affc9850ddb3cd433350e1cd6540048bc78ccd1085a478dc905a62bd64 in /nats-server 
# Tue, 19 Apr 2022 05:27:09 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 05:27:09 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:27:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 05:27:10 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 05:27:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b93faeabffe266939f160859e4fe954b65004d463416d6c943b83f17ea1a07c7`  
		Last Modified: Tue, 19 Apr 2022 05:29:29 GMT  
		Size: 4.2 MB (4229895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa486673456029146cdeb5aa24b79d59fbb46ceae19c2085f244a4f540a936c3`  
		Last Modified: Tue, 19 Apr 2022 05:29:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:92166da3897fa629b266a687308aee6da5d6a56a53a7b7bfd11009d8fec7c832
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4215629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622c4d607a2904fcea14a3b16b7c03c48cdbdc478a0d97fd80e79d6748b2767d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Apr 2022 03:28:46 GMT
COPY file:05c214eeb4e75353a7b7b920d3a6c8e8ae2768c0f9d965745307feda489dfdf1 in /nats-server 
# Tue, 19 Apr 2022 03:28:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 19 Apr 2022 03:28:47 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 19 Apr 2022 03:28:49 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 19 Apr 2022 03:28:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c1abcb1fd5645c2333d0ec9f6ffab7e85b00554c29b70f6bfc2d8d18b9e8bb2`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 4.2 MB (4215121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c98a93bee8cca0be2d741c7d90d5de238ba658cba0c41f37b42566e08a0442`  
		Last Modified: Tue, 19 Apr 2022 03:30:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:030f5e0b14dd2a887d63dee2637d561908c6b08b42893650326f58b254f02d6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:14bce2694d8e8899df545a7cd3547807dc2c2a8e62966e52c605e542d703127c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721251874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3be92f33ebc50102c9a1860e211aef8f924eb1aa14dc2803038ec9f991ecbf25`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 14:42:30 GMT
ENV NATS_DOCKERIZED=1
# Tue, 19 Apr 2022 01:23:43 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:23:44 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.0/nats-server-v2.8.0-windows-amd64.zip
# Tue, 19 Apr 2022 01:23:45 GMT
ENV NATS_SERVER_SHASUM=045e19fb61f60f7d7271e21c40e29ed5c746728ffb2acd5845e400d870887e11
# Tue, 19 Apr 2022 01:24:44 GMT
RUN Set-PSDebug -Trace 2
# Tue, 19 Apr 2022 01:26:17 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 19 Apr 2022 01:26:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 19 Apr 2022 01:26:19 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:26:20 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 19 Apr 2022 01:26:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d838c7a98a95bee63894bac798124e8c8572bcacc23e22d85332d453a03a7d7c`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d3e3a79bb829d65cf7ed61b8c2cf8350a6a7a405b3347adff7292297767eb`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cebc0769c427eb543681b030454f92d0ffbce74f8627c92b67203e4124d39`  
		Last Modified: Tue, 19 Apr 2022 01:27:16 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562c9b40b5a279e5d877b919b322f30e14d198b4a11bf5afa6eac87919d9ca24`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0dbc72a81b334128cf38a05560033f74cde85aae7c552dc95a76cc4005974`  
		Last Modified: Tue, 19 Apr 2022 01:27:15 GMT  
		Size: 359.3 KB (359323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3544837af17ae4efb8e835018cc439af97e5682c3f869bd8afa198bdbd7e577e`  
		Last Modified: Tue, 19 Apr 2022 01:27:14 GMT  
		Size: 5.0 MB (4958917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1a03a805566bb6dcdac96008842da65570c50929fcad33ad76b768b4a98d8`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fa9aab15861532a563a27d917f24e365ec71037a9ce79db53c6d9ccdae1225`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5989cf5455ac5bcad0bfcbef4c8374e05fc5b2fab25f348b6f14db27c627b04`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf354e75d471ae1f5ade3e00fcbf1d1da1e0096ae62fb81e7f014954220af0fe`  
		Last Modified: Tue, 19 Apr 2022 01:27:13 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
