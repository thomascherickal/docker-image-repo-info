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
-	[`nats:2.7.4`](#nats274)
-	[`nats:2.7.4-alpine`](#nats274-alpine)
-	[`nats:2.7.4-alpine3.15`](#nats274-alpine315)
-	[`nats:2.7.4-linux`](#nats274-linux)
-	[`nats:2.7.4-nanoserver`](#nats274-nanoserver)
-	[`nats:2.7.4-nanoserver-1809`](#nats274-nanoserver-1809)
-	[`nats:2.7.4-scratch`](#nats274-scratch)
-	[`nats:2.7.4-windowsservercore`](#nats274-windowsservercore)
-	[`nats:2.7.4-windowsservercore-1809`](#nats274-windowsservercore-1809)
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
$ docker pull nats@sha256:6f86d5bac0f78b01cf5f9f707008403b0792ff5029817f8afc23c895c5215cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

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

### `nats:2` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
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
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
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
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7`

```console
$ docker pull nats@sha256:6f86d5bac0f78b01cf5f9f707008403b0792ff5029817f8afc23c895c5215cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7` - linux; amd64

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

### `nats:2.7` - linux; arm variant v6

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

### `nats:2.7` - linux; arm variant v7

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

### `nats:2.7` - linux; arm64 variant v8

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

### `nats:2.7` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-alpine3.15`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-linux`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-linux` - linux; amd64

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

### `nats:2.7-linux` - linux; arm variant v6

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

### `nats:2.7-linux` - linux; arm variant v7

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

### `nats:2.7-linux` - linux; arm64 variant v8

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

## `nats:2.7-nanoserver`

```console
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-nanoserver-1809`

```console
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-scratch`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7-scratch` - linux; amd64

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

### `nats:2.7-scratch` - linux; arm variant v6

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

### `nats:2.7-scratch` - linux; arm variant v7

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

### `nats:2.7-scratch` - linux; arm64 variant v8

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

## `nats:2.7-windowsservercore`

```console
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7-windowsservercore-1809`

```console
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4`

```console
$ docker pull nats@sha256:6f86d5bac0f78b01cf5f9f707008403b0792ff5029817f8afc23c895c5215cc6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7.4` - linux; amd64

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

### `nats:2.7.4` - linux; arm variant v6

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

### `nats:2.7.4` - linux; arm variant v7

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

### `nats:2.7.4` - linux; arm64 variant v8

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

### `nats:2.7.4` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-alpine`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-alpine3.15`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.4-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.7.4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-linux`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.4-linux` - linux; amd64

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

### `nats:2.7.4-linux` - linux; arm variant v6

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

### `nats:2.7.4-linux` - linux; arm variant v7

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

### `nats:2.7.4-linux` - linux; arm64 variant v8

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

## `nats:2.7.4-nanoserver`

```console
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7.4-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-nanoserver-1809`

```console
$ docker pull nats@sha256:9654461ee3015e4abac8d6f24720ec089a72db6650768ac224cd6280735a70f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7.4-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:6d00c243dc589b03baf20fbe8c0a81279a5725d0774b275bbb9c3ebe329b570e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107611006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888ad60fdeb9e43dbbe336530422e503f539089048145cc1bbea7e51905b7095`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:16:59 GMT
RUN cmd /S /C #(nop) COPY file:741c07610cba7dd6badafc477fe411065386e3878f26a0bf50ed1d89036d6dcf in C:\nats-server.exe 
# Wed, 09 Mar 2022 23:17:00 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:17:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:17:02 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e02f868f2bb74e07262227b1156e17be47c4d960be7e9270cca8bc1dc6635b`  
		Last Modified: Wed, 09 Mar 2022 23:17:53 GMT  
		Size: 4.6 MB (4550038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9514eaf2c4a0d45ed2033bb85089d1fa90e61da7d517358225b5c6739051fcd7`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497be159edf0b99569392570b882cb48a2e72386befcbe1a0f454c6c02dba990`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c889054d0bd6db85b4b9c71958f5f7b8a6679ee127a701a521ee74961a3a528`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10493cee89e77ec8ec7093f8359147e7040171cbe811996808f6f1b860c78db`  
		Last Modified: Wed, 09 Mar 2022 23:17:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-scratch`

```console
$ docker pull nats@sha256:162126c602bcb3293ff5401b486cba4da6a3df5ed3b28758b1e9b11faeb382e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.7.4-scratch` - linux; amd64

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

### `nats:2.7.4-scratch` - linux; arm variant v6

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

### `nats:2.7.4-scratch` - linux; arm variant v7

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

### `nats:2.7.4-scratch` - linux; arm64 variant v8

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

## `nats:2.7.4-windowsservercore`

```console
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7.4-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.7.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:de7fa8eefd8b38a00c8f113294fc03f91486cde9b572b109e98f44f2ffbf5b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:2.7.4-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:ebc084a1a8e19ddf44701886869f9009dccaf6485d52d791799326d6f89ab0d2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720689430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f84a261eca9a7469f56f24e432d4ea475732107a3ab4cf28174ee49e3ba364b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 23:14:16 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:14:17 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.4/nats-server-v2.7.4-windows-amd64.zip
# Wed, 09 Mar 2022 23:14:18 GMT
ENV NATS_SERVER_SHASUM=0c98c505391e781f5f528817099dc727d83c997b3d48032c0f111d1452e8489b
# Wed, 09 Mar 2022 23:15:14 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 23:16:39 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 23:16:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 23:16:40 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:16:41 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 23:16:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e780f30b10c083782e0d53ed487fd4d8f8d32ad6c9b9fd84d2fcc0745ee60`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee7e8b0a6cef1b2ea81fcb039bc420172f4a60c3f329e6b495f9e1133e3e1534`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844fdd93ebcdfae84a099cefa8da35deaa056bff22b968bebf99205facdf928f`  
		Last Modified: Wed, 09 Mar 2022 23:17:33 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f545db8b309b5166354fd80028d4bda3d85af353da1959ab615769a430d1c0`  
		Last Modified: Wed, 09 Mar 2022 23:17:34 GMT  
		Size: 348.6 KB (348621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502abb43626a3eb4c75cb441213dbb73cbb7b0df0b28ff4d77b4420ebeb536e9`  
		Last Modified: Wed, 09 Mar 2022 23:17:36 GMT  
		Size: 4.9 MB (4874834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cef267e6b969aa61db520018b018b4244a92bbceda7eba76208a24bf2bcfbaf`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57f349791c768e9ea1eaf48b6c342b2038779b4cdca397333cc20c73ded703`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06857fcc2d8c8a67e6e493c5d95e54a6bded7af6103d139e4a59072664088bff`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62c41a5b49cd11c0da902b5333c829bcc21ffcb561d931fc457eafa36ee6bc9`  
		Last Modified: Wed, 09 Mar 2022 23:17:31 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:e1c68ff8dcfd80aeea74468aeab8313f8b72527ae7a5f6d5ef981d8838374406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:ae7411548aaccfbe8c77b0f055c26ca31e0f446b32d5e0ac2057d071c679adab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b6a6dceb55e0491347710d70c05fd4b3b0d1dd934735ee223c09b9d9fea2a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:25:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:25:44 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:25:44 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411cb49714978e9fd36e386ac31e6ee14d69e6d14ee4a135a9237c1478d9377a`  
		Last Modified: Wed, 09 Mar 2022 22:26:16 GMT  
		Size: 4.8 MB (4783191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4773cddf46de02d8766097101aadbeb05e4b7db6eda36123928f09f38cae8df8`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b3be5f66319a6729632a74114412f6c1bd9faf440593d17f331ce459515f5`  
		Last Modified: Wed, 09 Mar 2022 22:26:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:e49f7aeb99dcd7ac3d0b25c0a538c9f8a366631426d75f51ebb1b2573d02f583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7080038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9315428d3738da4f3b50407e1d2ff01a83584c29917c6673755083f0c9fb8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:05:34 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:05:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:05:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:05:39 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:05:40 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02be98e3c2fbd0e1f3bd3b8bc533fe01b7bf5fa4978696b99f4b1ac39cb188`  
		Last Modified: Wed, 09 Mar 2022 23:07:45 GMT  
		Size: 4.4 MB (4447615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48222a3442564d398d51fb3466073e46468a7f0982ce2d75c2b439748b884f14`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e76e49acfd137449ee5c2d205e64367307b30dc1fefc183354c6c95bb8ab7f3`  
		Last Modified: Wed, 09 Mar 2022 23:07:42 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:8c7fd43562ccda4c6517a4d48fad0de740d05feda37588e039e0e2d3ed6ab858
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6877147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd85ff8ccc13ba354c65e02ae670a2c45df663fcf9f501bef7d535a8e983d19c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 23:25:42 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 23:25:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 23:25:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 23:25:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 23:25:47 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:25:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 23:25:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c6bddd723a072d63982ab51a8b09cfdd40204c79987d352e51122cb4fdc0b8`  
		Last Modified: Wed, 09 Mar 2022 23:27:56 GMT  
		Size: 4.4 MB (4441380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d41c86b8f5d7d7b8c15a3ee2a504a6e4ddbee48eb60b579d7faa7a5b2101b5a`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ecf08180d84c0eedb8581c4c3606fd5ce6e48bf6191d1b3ca2f9271b851062`  
		Last Modified: Wed, 09 Mar 2022 23:27:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:79a5506cc66d2a0a1213dac8ba90a8d238e41527cebe5d680e2c2623726765c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7142790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab49aefb786a251205806da4d566eb13b4f51c8e79047bbb5746ba1a8b3c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Mar 2022 22:56:57 GMT
ENV NATS_SERVER=2.7.4
# Wed, 09 Mar 2022 22:56:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 09 Mar 2022 22:57:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 09 Mar 2022 22:57:02 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 09 Mar 2022 22:57:02 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Mar 2022 22:57:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedbb7879da3cfe5e29ede2bd47e93ab47323d734365ef6d7e327b6633440e2`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 4.4 MB (4426384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289bb7f1aee3e5693bd53dace086e0956ab5b54b7a3744ce58a82ad34c0f8a8d`  
		Last Modified: Wed, 09 Mar 2022 22:58:05 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745044e52b484df04288e6be0de1e2c774491e213e2fb48015bdfb93287a12d`  
		Last Modified: Wed, 09 Mar 2022 22:58:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:d04955d00da77dd90bf004ddacebb2967a96294a5f46f7637cb787001fee745e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2686; amd64

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
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
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

### `nats:latest` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:90209bda1cad3ec772bc2677672f501958ee7d62c33edfa857dc1716bda9220b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107602854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07847f304e7f8ec4f2b589a503ef48b8ec40f915777bb525440734cb80354bfe`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 16:40:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 16:40:12 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 16:40:13 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa5157704c1d4e58658a58ee4a6c9c9311a1d1fad5bed72177cbe21cf41dcb`  
		Last Modified: Wed, 09 Mar 2022 16:41:04 GMT  
		Size: 4.5 MB (4541860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa65daf1bc9817f903056d7a32becb96a3c4ae626707c391c115f9672dd19f9`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ca210f6c322c3169919cabf4b4814ab663aa766949d78aa18e5e52bbc9c7b7`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa906eba8a8100c8da6161e182387637cb7d3e7272ba27fb859f8c511abc7ba4`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a943f384f132c325e714fb870d67abbfbde1e4ffb1379784d990e39e0e3913`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:c5138097a7d91355c8ea3cb82b11f0bcdabae08a57191b7e0249b4322240385a
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
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
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
$ docker pull nats@sha256:17a7ba92d7d9e30b2ade1940d64a5f64ea45274342f23bce8aec50f7c7c0079a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:90209bda1cad3ec772bc2677672f501958ee7d62c33edfa857dc1716bda9220b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107602854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07847f304e7f8ec4f2b589a503ef48b8ec40f915777bb525440734cb80354bfe`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 16:40:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 16:40:12 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 16:40:13 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa5157704c1d4e58658a58ee4a6c9c9311a1d1fad5bed72177cbe21cf41dcb`  
		Last Modified: Wed, 09 Mar 2022 16:41:04 GMT  
		Size: 4.5 MB (4541860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa65daf1bc9817f903056d7a32becb96a3c4ae626707c391c115f9672dd19f9`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ca210f6c322c3169919cabf4b4814ab663aa766949d78aa18e5e52bbc9c7b7`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa906eba8a8100c8da6161e182387637cb7d3e7272ba27fb859f8c511abc7ba4`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a943f384f132c325e714fb870d67abbfbde1e4ffb1379784d990e39e0e3913`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:17a7ba92d7d9e30b2ade1940d64a5f64ea45274342f23bce8aec50f7c7c0079a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:90209bda1cad3ec772bc2677672f501958ee7d62c33edfa857dc1716bda9220b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107602854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07847f304e7f8ec4f2b589a503ef48b8ec40f915777bb525440734cb80354bfe`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Wed, 09 Mar 2022 16:40:09 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Wed, 09 Mar 2022 16:40:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 16:40:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 16:40:12 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 16:40:13 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6bc8e7abd2b889d7f3d81ab72c0dc6f44c22859ff125c228ec1147cd803c7e6c`  
		Last Modified: Wed, 09 Mar 2022 16:41:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faa5157704c1d4e58658a58ee4a6c9c9311a1d1fad5bed72177cbe21cf41dcb`  
		Last Modified: Wed, 09 Mar 2022 16:41:04 GMT  
		Size: 4.5 MB (4541860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa65daf1bc9817f903056d7a32becb96a3c4ae626707c391c115f9672dd19f9`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ca210f6c322c3169919cabf4b4814ab663aa766949d78aa18e5e52bbc9c7b7`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa906eba8a8100c8da6161e182387637cb7d3e7272ba27fb859f8c511abc7ba4`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a943f384f132c325e714fb870d67abbfbde1e4ffb1379784d990e39e0e3913`  
		Last Modified: Wed, 09 Mar 2022 16:40:59 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:c5138097a7d91355c8ea3cb82b11f0bcdabae08a57191b7e0249b4322240385a
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
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
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
$ docker pull nats@sha256:73e27c192194143e9b62c4f2ded2984b5675129b8657d9736845bcce6621cfc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:e1ff01e9229d5c7bec881c29fbeb094ef95b03e54a80f66f0e65fbe41a33bb4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720683253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd5fd97f45903baa3340c5695af50b2d1ed687b8a10e52d1f64d26c98161a5f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 16:36:40 GMT
ENV NATS_SERVER=2.7.3
# Wed, 09 Mar 2022 16:36:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Wed, 09 Mar 2022 16:36:42 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Wed, 09 Mar 2022 16:38:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 16:39:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 16:39:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 16:39:53 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 16:39:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 16:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e42c5b8ce3d2860dee66c1b5a94f8984a7164e8821a7730b2a2f3ae2ab3574`  
		Last Modified: Wed, 09 Mar 2022 16:40:42 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf812b1cfcec29602d107bef7e05f2c42661e6de68d06f42a6a50444bdfe0cb`  
		Last Modified: Wed, 09 Mar 2022 16:40:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4408e08c023d4b1c45f075bfdf96f67d7f0e09376be774314dd45c56ab1bd01d`  
		Last Modified: Wed, 09 Mar 2022 16:40:43 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d548cdcfc93bc734d4de576e696a2cdd3088415d58fedc3b9888e2a8a8c9e4b`  
		Last Modified: Wed, 09 Mar 2022 16:40:43 GMT  
		Size: 349.8 KB (349760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44951b18faf73d172b09675cbb05b8f9da0d304fa69141e9c317015e2126a6`  
		Last Modified: Wed, 09 Mar 2022 16:40:41 GMT  
		Size: 4.9 MB (4867494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc91fe37c5dfe9f191cd5f4612758e1dd9320b570ab236f45b76afa49a16b7b`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c93c11781e7cd21ad6b3b0eec7bc6a86e0c9076512fe83fb39f3c9eab62a05`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b639b85df7a056548a52711dfe322991b5fe92f311037f385e9788ffe8ae1aa4`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8667684816445549d2ee046f4686fd6e753de7ecebcedb42f8e517fff3989fbd`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:73e27c192194143e9b62c4f2ded2984b5675129b8657d9736845bcce6621cfc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull nats@sha256:e1ff01e9229d5c7bec881c29fbeb094ef95b03e54a80f66f0e65fbe41a33bb4f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720683253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd5fd97f45903baa3340c5695af50b2d1ed687b8a10e52d1f64d26c98161a5f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 16:36:38 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Mar 2022 16:36:40 GMT
ENV NATS_SERVER=2.7.3
# Wed, 09 Mar 2022 16:36:41 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.7.3/nats-server-v2.7.3-windows-amd64.zip
# Wed, 09 Mar 2022 16:36:42 GMT
ENV NATS_SERVER_SHASUM=ddb372da68741d897006c8d4b160c7f4788603cbaacb3fa105ddf7baada04428
# Wed, 09 Mar 2022 16:38:04 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Mar 2022 16:39:51 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Mar 2022 16:39:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Mar 2022 16:39:53 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 16:39:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Mar 2022 16:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431f904a213b56f70ee2943fb5c2ed2f4bcc65a509c6d79fce7ff98cfdfb4956`  
		Last Modified: Wed, 09 Mar 2022 16:40:44 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e42c5b8ce3d2860dee66c1b5a94f8984a7164e8821a7730b2a2f3ae2ab3574`  
		Last Modified: Wed, 09 Mar 2022 16:40:42 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf812b1cfcec29602d107bef7e05f2c42661e6de68d06f42a6a50444bdfe0cb`  
		Last Modified: Wed, 09 Mar 2022 16:40:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4408e08c023d4b1c45f075bfdf96f67d7f0e09376be774314dd45c56ab1bd01d`  
		Last Modified: Wed, 09 Mar 2022 16:40:43 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d548cdcfc93bc734d4de576e696a2cdd3088415d58fedc3b9888e2a8a8c9e4b`  
		Last Modified: Wed, 09 Mar 2022 16:40:43 GMT  
		Size: 349.8 KB (349760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44951b18faf73d172b09675cbb05b8f9da0d304fa69141e9c317015e2126a6`  
		Last Modified: Wed, 09 Mar 2022 16:40:41 GMT  
		Size: 4.9 MB (4867494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc91fe37c5dfe9f191cd5f4612758e1dd9320b570ab236f45b76afa49a16b7b`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c93c11781e7cd21ad6b3b0eec7bc6a86e0c9076512fe83fb39f3c9eab62a05`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b639b85df7a056548a52711dfe322991b5fe92f311037f385e9788ffe8ae1aa4`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8667684816445549d2ee046f4686fd6e753de7ecebcedb42f8e517fff3989fbd`  
		Last Modified: Wed, 09 Mar 2022 16:40:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
