<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.19`](#nats2919)
-	[`nats:2.9.19-alpine`](#nats2919-alpine)
-	[`nats:2.9.19-alpine3.18`](#nats2919-alpine318)
-	[`nats:2.9.19-linux`](#nats2919-linux)
-	[`nats:2.9.19-nanoserver`](#nats2919-nanoserver)
-	[`nats:2.9.19-nanoserver-1809`](#nats2919-nanoserver-1809)
-	[`nats:2.9.19-scratch`](#nats2919-scratch)
-	[`nats:2.9.19-windowsservercore`](#nats2919-windowsservercore)
-	[`nats:2.9.19-windowsservercore-1809`](#nats2919-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:518d0d3cd18c8449f21f881be81753f79dddee9864bd1db704880f70af36143e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:518d0d3cd18c8449f21f881be81753f79dddee9864bd1db704880f70af36143e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19`

```console
$ docker pull nats@sha256:518d0d3cd18c8449f21f881be81753f79dddee9864bd1db704880f70af36143e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.19` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-alpine`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.19-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-alpine3.18`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.19-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-linux`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.19-linux` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-nanoserver`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.19-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-nanoserver-1809`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.19-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-scratch`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.19-scratch` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.19-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-windowsservercore`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.19-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.19-windowsservercore-1809`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.19-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:8e6c8ac6ad5fa81da4206443a11ad86c24be63f08a11e17acc96636dc37401cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:79f55e1e1ac530428b0f3dbb8447fca8eb73d43b8706ea60041b9150ec9cee4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8807112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba37671be303876cc9cfaabde62d4cba45e69f890335b8257195f1d6109e6dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:17:25 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:17:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:17:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:17:28 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:17:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c14de251df13ed7d21c47cd279de1e6909afcd92ef08e3e220bd21826ad17c`  
		Last Modified: Wed, 21 Jun 2023 00:17:52 GMT  
		Size: 5.4 MB (5408233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae5c74d1f37b02a1a518849fb5ff1a7392f336d60cc3e120d74cb26088a6d29`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59566e38ec7be6b427690697eb98acbd97024ac5167a328a1a9110fd5336e0a`  
		Last Modified: Wed, 21 Jun 2023 00:17:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f5f7c93bd585c369a20c4771bd574b06477b67cf72f7805cc825839ba02242af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5dc3f5d44488dee7b308a8237dd9c89d5e801e27b56f0ac62a35ea3be1c365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Tue, 20 Jun 2023 23:49:17 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 20 Jun 2023 23:49:20 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 20 Jun 2023 23:49:20 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 20 Jun 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10ba3e7349b82995b9dde69255050db5f1aac6dd8580f9d80e33f4c3041920f`  
		Last Modified: Tue, 20 Jun 2023 23:49:48 GMT  
		Size: 5.2 MB (5170328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f2659e588d93ec57bb35c7a4358dcd188d290d2986a29252bb1578c0e49ed7`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8c97d99d294d23627872f107668b38afaf30b3f2eda9f09921823af4edd9cc`  
		Last Modified: Tue, 20 Jun 2023 23:49:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:d42b0952c95fca686f67910c9d8a3ff062e23acd1d4c4c9483d76ccd4dd64ece
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8062747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b15157ab7b8a856d3975e26cbd3060310e1a35b03d8b71922d703b1881b7c17e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:09:15 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:09:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:09:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:09:18 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:09:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b84fd19835fa4d25a00aefb9a29fa58064bef400cadb46dca4379f51aea9df`  
		Last Modified: Wed, 21 Jun 2023 00:09:52 GMT  
		Size: 5.2 MB (5163241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9babea9cb5c03c0b3ad9c273223967b0c7f601ee8f1266264673cc982ac707`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3febf8d9d1012edf70b3b51d8aee72c564d0623ebb8510a037dfb86bf735a`  
		Last Modified: Wed, 21 Jun 2023 00:09:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9d7047e7aa327735a497636a2a565c497ecdab4d39542b36d311378c6e66fa6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8302354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0290494870a431e33a0ddcacc6f8ad9b9ce8b9b4908f16c8e079756ea205ed47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 21 Jun 2023 00:15:29 GMT
ENV NATS_SERVER=2.9.19
# Wed, 21 Jun 2023 00:15:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='74d01dff16360fd4187f56005d1ca9783762e6693cc26ab015c73bddf1d02e48' ;; 		armhf) natsArch='arm6'; sha256='b8160af8d6585a97c7c794c1dffaba0429757b51654986d4e64de6b1ca64d457' ;; 		armv7) natsArch='arm7'; sha256='d2062448c98a907af83b2253c42b91a4cc98243f98e70f91a060d5eb94664dfe' ;; 		x86_64) natsArch='amd64'; sha256='e3856357cba44652776ade8de6fd0d6198d484f7b2419e97fbec6a9edfe84c49' ;; 		x86) natsArch='386'; sha256='a368c9f1456447093bc902fa2dffaaa1f282ed52a40cb2c4e015df80461b34a6' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 21 Jun 2023 00:15:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 21 Jun 2023 00:15:31 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 00:15:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb00d7e55df9bba47fe0634e06a979dae0fe0362c1eeac62da7dbc69bcec08c`  
		Last Modified: Wed, 21 Jun 2023 00:15:55 GMT  
		Size: 5.0 MB (4972110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18cbef28284265dd9e570b61ea0613ecd955c0cd58abf12d7b379e0db34eabf`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70361c011c7e732ec8545ea9382e6c492f07e92c784a78c9e8b526401dde5de7`  
		Last Modified: Wed, 21 Jun 2023 00:15:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:518d0d3cd18c8449f21f881be81753f79dddee9864bd1db704880f70af36143e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:8d996b07cbcec6886180d9bb44a16b613abc1e6bd5a78f80f320bf2110e6db7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:1cdac7722c97642bff78676bc86cf120f8a5552da7e93fe38ca5180b3767f508
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f11334743aead044ee0d78a9c73c14594e2834c2109e84bdc40b73920016b7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:1ecaf142bf3397672c19f4f7cafbde6022aab419425974af2f2bbda1c2330840 in C:\nats-server.exe 
# Tue, 20 Jun 2023 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3afc143449d1fb4ca46dde45deafb05b3ea1ea1ae4ff26abe5eeff04b4cad11`  
		Last Modified: Wed, 21 Jun 2023 00:16:08 GMT  
		Size: 5.2 MB (5174118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb549bc1b65979548a7950a917434656e2c97bd20cb09fa0cf7d5ed8a8ff655d`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e0c0df966a2c66f94e3836d370c06059990ada0e3ae529b7b7c12035850dd`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cc65560cec1421cd11aab36249616bfbc29758bc6a09a7566a4b8994a4b4f3`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dabb71653938f00ba554164823b5cf4b7889217a7b0aec795c7f0336cd59472`  
		Last Modified: Wed, 21 Jun 2023 00:16:07 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:4e043f1835eb142c588f83b2efba1e6f4fe71506c3ea0d06ceb8e55430a9e595
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:d16e1e48c0ab845192603492b3d9c64445983a3dc5667ec2d581f2870424d68f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca39502494bbde906154629d4c0a6e88389a16bf77d69e274587dd1dc8afa4c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:17:34 GMT
COPY file:0c5b3273ac56fdd9a548c5562dc6cca434baed1b8b5486460a64f797a00263af in /nats-server 
# Wed, 21 Jun 2023 00:17:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:17:35 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:17:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:17:35 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:17:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:41d97cbbc06ca3db7712fe594a3002518a211924b7a2a273d85c1aa8c1197696`  
		Last Modified: Wed, 21 Jun 2023 00:18:12 GMT  
		Size: 5.1 MB (5122205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2a4ef06e2a4e8f39e43fb44106a50476193b933ecaab0a1d6e582794dd5577`  
		Last Modified: Wed, 21 Jun 2023 00:18:11 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:dbf61af51cfb84bd3608b42332e5ae08ce2d5a791538f4a332f4c386daeb9ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4885319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca14db1f37a22c3c3605c951813c85b987e732d6f0f47452ebd64d91f111c83`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:ff9c6b5d5fd35fc16128c801a90e09fe72db48e42978c3e3899ecfd7236fe04e in /nats-server 
# Tue, 20 Jun 2023 23:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 20 Jun 2023 23:49:29 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:49:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 20 Jun 2023 23:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 20 Jun 2023 23:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:aae2ed191bc4bace1b4529b4f9854bc32c18be066a24d460e2aaf9c8a718c7b9`  
		Last Modified: Tue, 20 Jun 2023 23:50:09 GMT  
		Size: 4.9 MB (4884813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9406e57363ece1d3b6b8abfa39211ad7f0093d83837b484c5cc2c50912308f32`  
		Last Modified: Tue, 20 Jun 2023 23:50:08 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:55d0a97fd6b8545229214515f0b602829800d5945d91f12186e2abc4c905cfae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b98d9a7220cafc3414a842dc2edf402cd1530aa26574de19cfb6f21408a19b4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:01958cf912dc4ee20e8b0fb70a3d0de3d63643774adc3ae0be935d8d09c97dab in /nats-server 
# Wed, 21 Jun 2023 00:09:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:09:33 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:09:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:09:33 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:09:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:da6bffc650385dc011fd2a8b3128dbeca7a7660e2871df1f81f75ba119957e35`  
		Last Modified: Wed, 21 Jun 2023 00:10:13 GMT  
		Size: 4.9 MB (4876094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a780e691c52c3e5da4018a474c8645c2bdf15a579f4aa28abdc9df5bb929ff41`  
		Last Modified: Wed, 21 Jun 2023 00:10:11 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ab6dcfe06a1eee538235ba74c29c53d8fb2d46b7d053aee64b7f6d138ffced8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdf6eb10bb37d0efe11e788b04e433ccad9c0838b26bd4dfb8e84d03c3df4fa`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:6dc04ecbe26e2f3419cc32efecbab24e08c4e5e1159cf103444ed8297e83dfd6 in /nats-server 
# Wed, 21 Jun 2023 00:15:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 21 Jun 2023 00:15:38 GMT
EXPOSE 4222 6222 8222
# Wed, 21 Jun 2023 00:15:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 21 Jun 2023 00:15:38 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 21 Jun 2023 00:15:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:719bc06bdd9bd4c4c08d2f3030227de063dc2c6cfdbd8c4dee82757a9b32422d`  
		Last Modified: Wed, 21 Jun 2023 00:16:14 GMT  
		Size: 4.7 MB (4687741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8744977fbb1df9e2d0b8b2fd74ea3514e265be3ab31e4147897a9ec1c2274af`  
		Last Modified: Wed, 21 Jun 2023 00:16:13 GMT  
		Size: 504.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:c710fb3fec9750d89df471bbd2f245e00e6fa000a26ae502aa5f5f6d4c2322e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:8650676f605283a5a9b415e2e13bfa2c386a2f01a4c7069498e3b374a0e33214
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656422350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96db184fc44c52fe5dd68da11f75c71d405c97d2290a60122bebad2c4a877626`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Tue, 20 Jun 2023 23:15:16 GMT
ENV NATS_SERVER=2.9.19
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.19/nats-server-v2.9.19-windows-amd64.zip
# Tue, 20 Jun 2023 23:15:17 GMT
ENV NATS_SERVER_SHASUM=52f263cdc2748041011019bd988705a97340263bbd06615e70ac5c0aebfac2f0
# Tue, 20 Jun 2023 23:15:53 GMT
RUN Set-PSDebug -Trace 2
# Tue, 20 Jun 2023 23:16:46 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 20 Jun 2023 23:16:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 20 Jun 2023 23:16:47 GMT
EXPOSE 4222 6222 8222
# Tue, 20 Jun 2023 23:16:48 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 20 Jun 2023 23:16:49 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739eab246adff1610da5b3325e0aaa2f230e797a2a9d2e54f84a4d649fb85ce`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea84ea2cee2a86fd11d9f3d0ff636e50e3ced29d9608305a3724731859c3d54`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.3 KB (1274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330124d3567d24e424539bf8f7ab07d749dc8a42d0861091ed32b7858175bae`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952929309ab17e747fa7896b3b49db4aebf1b7e51f1281be46ff05266fa30ec`  
		Last Modified: Wed, 21 Jun 2023 00:15:53 GMT  
		Size: 320.7 KB (320734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0aab80c41559f6481cea6150a201e80dcec00bfca9fc94a220330ae875fb562`  
		Last Modified: Wed, 21 Jun 2023 00:15:52 GMT  
		Size: 5.5 MB (5468776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f1f0e4117098403a65fb95d52e0f4b56b65b41fdfc56ef40452bc5c14beb9e`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.8 KB (1849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90d67befbbe020a535d2ccfee7ccc67317ecd3d47fba3c6c830d1aab002a207`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3cdc1d1f3a5c3fed66d3ad909d2a4943ae9ffab331d36c89ed86084f4c83f7`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92917ae81744a0b659ce7d25b243a3ba490b162e55454f3890e8909dc4ef05f`  
		Last Modified: Wed, 21 Jun 2023 00:15:50 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
