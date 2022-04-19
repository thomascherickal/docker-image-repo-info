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
$ docker pull nats@sha256:3a55fa44c966259400450642b64197512a9b9144e8d995b710023c52bcbcb54f
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
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:b07b9411c2623fd623b1b2f0686a4c16409c7ee33a5823de00c471df9f3ff225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:bed4f10253c279b665399962dd8a61466115c3e1e9acd74470e29f955c4dc923
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7598738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e73e44dba4525c4492e520e3e4a1f9f6779f65392fd594fa2114e54056cf7a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:01:36 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 10:01:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 10:01:38 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 10:01:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:01:38 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a96228d46666e8b8ae2568e55f7acf4960e143037960b82918af20ea0819af`  
		Last Modified: Tue, 05 Apr 2022 10:02:10 GMT  
		Size: 4.8 MB (4783184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e69c23e316a0a475d94261816afea9a6f4a0cfee51c7a6a6f7b4bb58d6440b3`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b072d51df9425c0aa9c8247ca51d43b607a579e6d46c8e7525547cc4737e7`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5fc8fd7676645c7950099610debe9157c14465cb4f0f8bd351cbbc234cbc7aac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7070600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f391818b70f801bae97f808f994a7429d30dff883c0500c1747f25bd64075b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:52:08 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 14:52:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 14:52:14 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 14:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:52:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7706c52730f4cd1d72d74607ed59ccf0947aff065703de55f8c1788e37158d`  
		Last Modified: Tue, 05 Apr 2022 14:54:19 GMT  
		Size: 4.4 MB (4447625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f434c11aabbfe860f0ef3c58735c9276c99d596a6550a94fec9fcb12ed5d9c`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3510ad1e2456d3271b139cd96a5d8870e50d6f61442093a492e72f6073b9489a`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9340cbad2dc025179dc865f5c6f66a69096ded50b2e46afded61ac1f3b412cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6866697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f09ecdf2b0aff0fde7ed73027dbc749b7a657349415a11509ae32a4c900514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:55:26 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 15:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 15:55:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 15:55:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 15:55:31 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 15:55:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:55:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c97ae8e5682d5886f6ccd7ea053da726cc295b9f7293808d4b51ba06210713`  
		Last Modified: Tue, 05 Apr 2022 15:57:37 GMT  
		Size: 4.4 MB (4441372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66714d285cac5fb950706af50a1fbf277ce179d417ca4138c893811e75d820d8`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54375ec28ca00cc6542be4b669aefc6254266ed385d996ce0d2a870b373a4e19`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:939bee059703b05c5b0846c20b51fc00d2400e36f230c70ccbb00f7c5215791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067db6f9113d6046cb69c33eae58d0141981d3977f2ae17002944032bff6c30c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:55:12 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 08:55:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 08:55:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 08:55:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 08:55:18 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 08:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 08:55:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877eaed0217fc0aefecc8729fcaf3ce7f38ef83f37612dae5c7aebd817496b18`  
		Last Modified: Tue, 05 Apr 2022 08:56:19 GMT  
		Size: 4.4 MB (4426416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a426890e711d28c3849e31785f24b70e6931e1bf1c9aa838bc482ae377e0e7`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ff805262a2c8d64c4660b5f55697e58b27ca330d23f392be3fe262d2f2efd`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:b07b9411c2623fd623b1b2f0686a4c16409c7ee33a5823de00c471df9f3ff225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:bed4f10253c279b665399962dd8a61466115c3e1e9acd74470e29f955c4dc923
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7598738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e73e44dba4525c4492e520e3e4a1f9f6779f65392fd594fa2114e54056cf7a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:01:36 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 10:01:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 10:01:38 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 10:01:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:01:38 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a96228d46666e8b8ae2568e55f7acf4960e143037960b82918af20ea0819af`  
		Last Modified: Tue, 05 Apr 2022 10:02:10 GMT  
		Size: 4.8 MB (4783184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e69c23e316a0a475d94261816afea9a6f4a0cfee51c7a6a6f7b4bb58d6440b3`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b072d51df9425c0aa9c8247ca51d43b607a579e6d46c8e7525547cc4737e7`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:5fc8fd7676645c7950099610debe9157c14465cb4f0f8bd351cbbc234cbc7aac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7070600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f391818b70f801bae97f808f994a7429d30dff883c0500c1747f25bd64075b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:52:08 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 14:52:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 14:52:14 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 14:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:52:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7706c52730f4cd1d72d74607ed59ccf0947aff065703de55f8c1788e37158d`  
		Last Modified: Tue, 05 Apr 2022 14:54:19 GMT  
		Size: 4.4 MB (4447625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f434c11aabbfe860f0ef3c58735c9276c99d596a6550a94fec9fcb12ed5d9c`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3510ad1e2456d3271b139cd96a5d8870e50d6f61442093a492e72f6073b9489a`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:9340cbad2dc025179dc865f5c6f66a69096ded50b2e46afded61ac1f3b412cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6866697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f09ecdf2b0aff0fde7ed73027dbc749b7a657349415a11509ae32a4c900514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:55:26 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 15:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 15:55:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 15:55:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 15:55:31 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 15:55:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:55:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c97ae8e5682d5886f6ccd7ea053da726cc295b9f7293808d4b51ba06210713`  
		Last Modified: Tue, 05 Apr 2022 15:57:37 GMT  
		Size: 4.4 MB (4441372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66714d285cac5fb950706af50a1fbf277ce179d417ca4138c893811e75d820d8`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54375ec28ca00cc6542be4b669aefc6254266ed385d996ce0d2a870b373a4e19`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:939bee059703b05c5b0846c20b51fc00d2400e36f230c70ccbb00f7c5215791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067db6f9113d6046cb69c33eae58d0141981d3977f2ae17002944032bff6c30c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:55:12 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 08:55:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 08:55:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 08:55:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 08:55:18 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 08:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 08:55:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877eaed0217fc0aefecc8729fcaf3ce7f38ef83f37612dae5c7aebd817496b18`  
		Last Modified: Tue, 05 Apr 2022 08:56:19 GMT  
		Size: 4.4 MB (4426416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a426890e711d28c3849e31785f24b70e6931e1bf1c9aa838bc482ae377e0e7`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ff805262a2c8d64c4660b5f55697e58b27ca330d23f392be3fe262d2f2efd`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:338b160beda6c311f0a03bd19a96f5b0513d81ea04e4e2cd319b2db00d9f7218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:338b160beda6c311f0a03bd19a96f5b0513d81ea04e4e2cd319b2db00d9f7218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:1cf708930365988e84f38a615ae03baeda3bd2aacceaafc41df0f6f5243142ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:d0816612914e61b3aad1284fe48f848fe39031d67b5f7180afba9537c5e9841c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721182749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311c23a5f536bdab4938b0bf374d6303917df128f0943b269ecd86455cb28e5`
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
# Wed, 13 Apr 2022 14:42:31 GMT
ENV NATS_SERVER=2.7.4
# Wed, 13 Apr 2022 14:42:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 13 Apr 2022 14:42:33 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 13 Apr 2022 14:43:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Apr 2022 14:45:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Apr 2022 14:45:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:21 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:23 GMT
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
	-	`sha256:3a0657156d36069ff3139e7dcca912fdbb08ec7cb2bdd03bbda38b213815005d`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2600f244f19cd8b54cb88f22e09e7782722919ac4f4c951d6e3983c75b7f9c`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7557cc1e39a18eb0b77cdb3fa42f4e8ead64c4ddf5d9ee3b3eedf031b86f4a`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b27fbb9404f7e2f2077f3cfd782934861a012f169a86c7ff00258a2bc6d56`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 359.5 KB (359504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44575ccaa566365cd7c2e94979c3a8c125e713bd987104aa3d7b2eaedc21bb5`  
		Last Modified: Wed, 13 Apr 2022 14:46:15 GMT  
		Size: 4.9 MB (4889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95149c441f2dd97c433cd69c77b236d43a8fb6f8bb8836619a044144a1178e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 2.0 KB (2008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd923cdce2e70a45cd8de7e5f0d5cfde0566449b8f64dfa93b67d0dfc867179f`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a533af79a712ad124da5093f5716da36615d5e502340200674230b8de3a1b8e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fb08d905e270c20aa87ff7a06cdb619eb3c8a1493264c7560e8dd69556a19d`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:1cf708930365988e84f38a615ae03baeda3bd2aacceaafc41df0f6f5243142ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:d0816612914e61b3aad1284fe48f848fe39031d67b5f7180afba9537c5e9841c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721182749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311c23a5f536bdab4938b0bf374d6303917df128f0943b269ecd86455cb28e5`
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
# Wed, 13 Apr 2022 14:42:31 GMT
ENV NATS_SERVER=2.7.4
# Wed, 13 Apr 2022 14:42:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 13 Apr 2022 14:42:33 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 13 Apr 2022 14:43:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Apr 2022 14:45:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Apr 2022 14:45:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:21 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:23 GMT
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
	-	`sha256:3a0657156d36069ff3139e7dcca912fdbb08ec7cb2bdd03bbda38b213815005d`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2600f244f19cd8b54cb88f22e09e7782722919ac4f4c951d6e3983c75b7f9c`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7557cc1e39a18eb0b77cdb3fa42f4e8ead64c4ddf5d9ee3b3eedf031b86f4a`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b27fbb9404f7e2f2077f3cfd782934861a012f169a86c7ff00258a2bc6d56`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 359.5 KB (359504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44575ccaa566365cd7c2e94979c3a8c125e713bd987104aa3d7b2eaedc21bb5`  
		Last Modified: Wed, 13 Apr 2022 14:46:15 GMT  
		Size: 4.9 MB (4889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95149c441f2dd97c433cd69c77b236d43a8fb6f8bb8836619a044144a1178e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 2.0 KB (2008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd923cdce2e70a45cd8de7e5f0d5cfde0566449b8f64dfa93b67d0dfc867179f`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a533af79a712ad124da5093f5716da36615d5e502340200674230b8de3a1b8e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fb08d905e270c20aa87ff7a06cdb619eb3c8a1493264c7560e8dd69556a19d`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

**does not exist** (yet?)

## `nats:2.8-alpine`

**does not exist** (yet?)

## `nats:2.8-alpine3.15`

**does not exist** (yet?)

## `nats:2.8-linux`

**does not exist** (yet?)

## `nats:2.8-nanoserver`

**does not exist** (yet?)

## `nats:2.8-nanoserver-1809`

**does not exist** (yet?)

## `nats:2.8-scratch`

**does not exist** (yet?)

## `nats:2.8-windowsservercore`

**does not exist** (yet?)

## `nats:2.8-windowsservercore-1809`

**does not exist** (yet?)

## `nats:2.8.0`

**does not exist** (yet?)

## `nats:2.8.0-alpine`

**does not exist** (yet?)

## `nats:2.8.0-alpine3.15`

**does not exist** (yet?)

## `nats:2.8.0-linux`

**does not exist** (yet?)

## `nats:2.8.0-nanoserver`

**does not exist** (yet?)

## `nats:2.8.0-nanoserver-1809`

**does not exist** (yet?)

## `nats:2.8.0-scratch`

**does not exist** (yet?)

## `nats:2.8.0-windowsservercore`

**does not exist** (yet?)

## `nats:2.8.0-windowsservercore-1809`

**does not exist** (yet?)

## `nats:alpine`

```console
$ docker pull nats@sha256:b07b9411c2623fd623b1b2f0686a4c16409c7ee33a5823de00c471df9f3ff225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:bed4f10253c279b665399962dd8a61466115c3e1e9acd74470e29f955c4dc923
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7598738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e73e44dba4525c4492e520e3e4a1f9f6779f65392fd594fa2114e54056cf7a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:01:36 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 10:01:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 10:01:38 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 10:01:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:01:38 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a96228d46666e8b8ae2568e55f7acf4960e143037960b82918af20ea0819af`  
		Last Modified: Tue, 05 Apr 2022 10:02:10 GMT  
		Size: 4.8 MB (4783184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e69c23e316a0a475d94261816afea9a6f4a0cfee51c7a6a6f7b4bb58d6440b3`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b072d51df9425c0aa9c8247ca51d43b607a579e6d46c8e7525547cc4737e7`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5fc8fd7676645c7950099610debe9157c14465cb4f0f8bd351cbbc234cbc7aac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7070600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f391818b70f801bae97f808f994a7429d30dff883c0500c1747f25bd64075b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:52:08 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 14:52:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 14:52:14 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 14:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:52:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7706c52730f4cd1d72d74607ed59ccf0947aff065703de55f8c1788e37158d`  
		Last Modified: Tue, 05 Apr 2022 14:54:19 GMT  
		Size: 4.4 MB (4447625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f434c11aabbfe860f0ef3c58735c9276c99d596a6550a94fec9fcb12ed5d9c`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3510ad1e2456d3271b139cd96a5d8870e50d6f61442093a492e72f6073b9489a`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9340cbad2dc025179dc865f5c6f66a69096ded50b2e46afded61ac1f3b412cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6866697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f09ecdf2b0aff0fde7ed73027dbc749b7a657349415a11509ae32a4c900514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:55:26 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 15:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 15:55:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 15:55:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 15:55:31 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 15:55:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:55:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c97ae8e5682d5886f6ccd7ea053da726cc295b9f7293808d4b51ba06210713`  
		Last Modified: Tue, 05 Apr 2022 15:57:37 GMT  
		Size: 4.4 MB (4441372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66714d285cac5fb950706af50a1fbf277ce179d417ca4138c893811e75d820d8`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54375ec28ca00cc6542be4b669aefc6254266ed385d996ce0d2a870b373a4e19`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:939bee059703b05c5b0846c20b51fc00d2400e36f230c70ccbb00f7c5215791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067db6f9113d6046cb69c33eae58d0141981d3977f2ae17002944032bff6c30c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:55:12 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 08:55:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 08:55:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 08:55:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 08:55:18 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 08:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 08:55:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877eaed0217fc0aefecc8729fcaf3ce7f38ef83f37612dae5c7aebd817496b18`  
		Last Modified: Tue, 05 Apr 2022 08:56:19 GMT  
		Size: 4.4 MB (4426416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a426890e711d28c3849e31785f24b70e6931e1bf1c9aa838bc482ae377e0e7`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ff805262a2c8d64c4660b5f55697e58b27ca330d23f392be3fe262d2f2efd`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:b07b9411c2623fd623b1b2f0686a4c16409c7ee33a5823de00c471df9f3ff225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:bed4f10253c279b665399962dd8a61466115c3e1e9acd74470e29f955c4dc923
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7598738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e73e44dba4525c4492e520e3e4a1f9f6779f65392fd594fa2114e54056cf7a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:01:36 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 10:01:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 10:01:38 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 10:01:38 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 10:01:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:01:38 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a96228d46666e8b8ae2568e55f7acf4960e143037960b82918af20ea0819af`  
		Last Modified: Tue, 05 Apr 2022 10:02:10 GMT  
		Size: 4.8 MB (4783184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e69c23e316a0a475d94261816afea9a6f4a0cfee51c7a6a6f7b4bb58d6440b3`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b072d51df9425c0aa9c8247ca51d43b607a579e6d46c8e7525547cc4737e7`  
		Last Modified: Tue, 05 Apr 2022 10:02:09 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:5fc8fd7676645c7950099610debe9157c14465cb4f0f8bd351cbbc234cbc7aac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7070600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f391818b70f801bae97f808f994a7429d30dff883c0500c1747f25bd64075b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 14:52:08 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 14:52:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 14:52:13 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 14:52:14 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 14:52:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:52:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7706c52730f4cd1d72d74607ed59ccf0947aff065703de55f8c1788e37158d`  
		Last Modified: Tue, 05 Apr 2022 14:54:19 GMT  
		Size: 4.4 MB (4447625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f434c11aabbfe860f0ef3c58735c9276c99d596a6550a94fec9fcb12ed5d9c`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3510ad1e2456d3271b139cd96a5d8870e50d6f61442093a492e72f6073b9489a`  
		Last Modified: Tue, 05 Apr 2022 14:54:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:9340cbad2dc025179dc865f5c6f66a69096ded50b2e46afded61ac1f3b412cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6866697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f09ecdf2b0aff0fde7ed73027dbc749b7a657349415a11509ae32a4c900514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:55:26 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 15:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 15:55:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 15:55:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 15:55:31 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 15:55:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:55:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c97ae8e5682d5886f6ccd7ea053da726cc295b9f7293808d4b51ba06210713`  
		Last Modified: Tue, 05 Apr 2022 15:57:37 GMT  
		Size: 4.4 MB (4441372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66714d285cac5fb950706af50a1fbf277ce179d417ca4138c893811e75d820d8`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54375ec28ca00cc6542be4b669aefc6254266ed385d996ce0d2a870b373a4e19`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:939bee059703b05c5b0846c20b51fc00d2400e36f230c70ccbb00f7c5215791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067db6f9113d6046cb69c33eae58d0141981d3977f2ae17002944032bff6c30c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:55:12 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 08:55:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 08:55:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 08:55:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 08:55:18 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 08:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 08:55:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877eaed0217fc0aefecc8729fcaf3ce7f38ef83f37612dae5c7aebd817496b18`  
		Last Modified: Tue, 05 Apr 2022 08:56:19 GMT  
		Size: 4.4 MB (4426416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a426890e711d28c3849e31785f24b70e6931e1bf1c9aa838bc482ae377e0e7`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ff805262a2c8d64c4660b5f55697e58b27ca330d23f392be3fe262d2f2efd`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:3a55fa44c966259400450642b64197512a9b9144e8d995b710023c52bcbcb54f
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
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:338b160beda6c311f0a03bd19a96f5b0513d81ea04e4e2cd319b2db00d9f7218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:338b160beda6c311f0a03bd19a96f5b0513d81ea04e4e2cd319b2db00d9f7218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:8f862dd6bae660425765780cdc271275a6fd0487a731be1ee22b48edb4be477d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.7 MB (107652289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ebe13c71286e0e75bccc444f6884d496f043c06be5e76f2fe4b31a852927bd0`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 14:45:42 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Apr 2022 14:45:43 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 13 Apr 2022 14:45:44 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:45 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:46 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:47 GMT
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
	-	`sha256:e390a1614c6e51a8b6427f7a28e408d5e7686ceac8399397a9e62357ae5e844d`  
		Last Modified: Wed, 13 Apr 2022 14:46:38 GMT  
		Size: 4.6 MB (4550075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756555742908471847260062ea575f5d1b2353f4b644f9e4ff80ab80b00486fe`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c129657727c02d0dac7e07e554140e188f4deb6e6270dd954b4c4d7198ca554`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72622f01880f0ece2286a64bca2116dfcf00642664c5f1b9171c6cce041318a7`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5faf58f7a1d30381ba2dd6e38f4b10d8b27d8064a2eec3f1f9205028422adfd0`  
		Last Modified: Wed, 13 Apr 2022 14:46:33 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ed87fc96ebeace8ad252ad368ab68f1ef976daadae90f50d8f1f917364b8050c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4169387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c348e474d9b30a28b01ce9d8566ee12c3404e1a91cddfa31c8de44ba3c6b495b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:26:11 GMT
COPY file:143b3802bb689cd4b4badd2b1463feaa3881f20e6fd303b203aa25ea206fb684 in /nats-server 
# Wed, 09 Mar 2022 23:26:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:26:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:26:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:26:13 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:26:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c0d2f46ac12a6f6109f1f810a72658a0faa0b7301dfa2abc4f222012bab43639`  
		Last Modified: Wed, 09 Mar 2022 23:28:32 GMT  
		Size: 4.2 MB (4168878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e39b35a6f91da4330c0e57dcc7c9e91270e4d54cf1097b98ad3ab1a1ca178`  
		Last Modified: Wed, 09 Mar 2022 23:28:29 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:1cf708930365988e84f38a615ae03baeda3bd2aacceaafc41df0f6f5243142ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:d0816612914e61b3aad1284fe48f848fe39031d67b5f7180afba9537c5e9841c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721182749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311c23a5f536bdab4938b0bf374d6303917df128f0943b269ecd86455cb28e5`
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
# Wed, 13 Apr 2022 14:42:31 GMT
ENV NATS_SERVER=2.7.4
# Wed, 13 Apr 2022 14:42:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 13 Apr 2022 14:42:33 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 13 Apr 2022 14:43:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Apr 2022 14:45:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Apr 2022 14:45:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:21 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:23 GMT
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
	-	`sha256:3a0657156d36069ff3139e7dcca912fdbb08ec7cb2bdd03bbda38b213815005d`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2600f244f19cd8b54cb88f22e09e7782722919ac4f4c951d6e3983c75b7f9c`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7557cc1e39a18eb0b77cdb3fa42f4e8ead64c4ddf5d9ee3b3eedf031b86f4a`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b27fbb9404f7e2f2077f3cfd782934861a012f169a86c7ff00258a2bc6d56`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 359.5 KB (359504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44575ccaa566365cd7c2e94979c3a8c125e713bd987104aa3d7b2eaedc21bb5`  
		Last Modified: Wed, 13 Apr 2022 14:46:15 GMT  
		Size: 4.9 MB (4889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95149c441f2dd97c433cd69c77b236d43a8fb6f8bb8836619a044144a1178e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 2.0 KB (2008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd923cdce2e70a45cd8de7e5f0d5cfde0566449b8f64dfa93b67d0dfc867179f`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a533af79a712ad124da5093f5716da36615d5e502340200674230b8de3a1b8e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fb08d905e270c20aa87ff7a06cdb619eb3c8a1493264c7560e8dd69556a19d`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:1cf708930365988e84f38a615ae03baeda3bd2aacceaafc41df0f6f5243142ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull nats@sha256:d0816612914e61b3aad1284fe48f848fe39031d67b5f7180afba9537c5e9841c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2721182749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f311c23a5f536bdab4938b0bf374d6303917df128f0943b269ecd86455cb28e5`
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
# Wed, 13 Apr 2022 14:42:31 GMT
ENV NATS_SERVER=2.7.4
# Wed, 13 Apr 2022 14:42:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 13 Apr 2022 14:42:33 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 13 Apr 2022 14:43:34 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Apr 2022 14:45:19 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Apr 2022 14:45:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Apr 2022 14:45:21 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Apr 2022 14:45:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Apr 2022 14:45:23 GMT
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
	-	`sha256:3a0657156d36069ff3139e7dcca912fdbb08ec7cb2bdd03bbda38b213815005d`  
		Last Modified: Wed, 13 Apr 2022 14:46:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2600f244f19cd8b54cb88f22e09e7782722919ac4f4c951d6e3983c75b7f9c`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7557cc1e39a18eb0b77cdb3fa42f4e8ead64c4ddf5d9ee3b3eedf031b86f4a`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877b27fbb9404f7e2f2077f3cfd782934861a012f169a86c7ff00258a2bc6d56`  
		Last Modified: Wed, 13 Apr 2022 14:46:16 GMT  
		Size: 359.5 KB (359504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44575ccaa566365cd7c2e94979c3a8c125e713bd987104aa3d7b2eaedc21bb5`  
		Last Modified: Wed, 13 Apr 2022 14:46:15 GMT  
		Size: 4.9 MB (4889678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f95149c441f2dd97c433cd69c77b236d43a8fb6f8bb8836619a044144a1178e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 2.0 KB (2008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd923cdce2e70a45cd8de7e5f0d5cfde0566449b8f64dfa93b67d0dfc867179f`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a533af79a712ad124da5093f5716da36615d5e502340200674230b8de3a1b8e`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fb08d905e270c20aa87ff7a06cdb619eb3c8a1493264c7560e8dd69556a19d`  
		Last Modified: Wed, 13 Apr 2022 14:46:14 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
