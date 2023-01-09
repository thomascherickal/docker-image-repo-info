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
-	[`nats:2.9.11`](#nats2911)
-	[`nats:2.9.11-alpine`](#nats2911-alpine)
-	[`nats:2.9.11-alpine3.17`](#nats2911-alpine317)
-	[`nats:2.9.11-linux`](#nats2911-linux)
-	[`nats:2.9.11-nanoserver`](#nats2911-nanoserver)
-	[`nats:2.9.11-nanoserver-1809`](#nats2911-nanoserver-1809)
-	[`nats:2.9.11-scratch`](#nats2911-scratch)
-	[`nats:2.9.11-windowsservercore`](#nats2911-windowsservercore)
-	[`nats:2.9.11-windowsservercore-1809`](#nats2911-windowsservercore-1809)
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
$ docker pull nats@sha256:3ba544a6bbef5767fb28be2737308833ea6f6fbddcb36cc0c8f42bef58ebaf33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:3ba544a6bbef5767fb28be2737308833ea6f6fbddcb36cc0c8f42bef58ebaf33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11`

```console
$ docker pull nats@sha256:3ba544a6bbef5767fb28be2737308833ea6f6fbddcb36cc0c8f42bef58ebaf33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9.11` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-alpine`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.11-alpine` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-alpine3.17`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.11-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-linux`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.11-linux` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-nanoserver`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9.11-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-nanoserver-1809`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9.11-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-scratch`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.11-scratch` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.11-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-windowsservercore`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9.11-windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.11-windowsservercore-1809`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:2.9.11-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:4dc871d9aa401561b2e058e60b80c7b5429abfe2363b2fb8e92aa7fc27ab3db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:1dd295a7f31f7eb78b3c129af22330e760aa82a0775ad0248c650affc7aebb00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8585788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2aa27f35c926d598c5c04c23cf06335ced5dc68a66e01d77cf283a9bf862763`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:34:19 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:34:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:34:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:34:22 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:34:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:34:22 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadfb97be2c4b396acd5dc611490acf3a27bb9035f500fd74398464a6eb65fca`  
		Last Modified: Mon, 09 Jan 2023 18:34:52 GMT  
		Size: 5.2 MB (5214165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbf89eaa7ee5ce3d2515cf4740199f17ff7ed06adcc9d89e5b3fd5db6015a1b`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c489337ee522622a844b9ef1c9436394534cd4a3d84fe9919e16cac43889c6a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:7f370073ed44501cc78760b1ad096230e3a48d5aa2ccf617dc2ad3b49816967a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8086974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5c7813b2266c292d24b2bc4e4e4d087b9cf371bb2bf42e0c5751d967a4504d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Fri, 06 Jan 2023 19:01:33 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:01:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 06 Jan 2023 19:01:37 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Jan 2023 19:01:37 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 19:01:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9c430594153fe16619545b3691109f69f6b50cf249e56cb38ab103cde91ad3`  
		Last Modified: Fri, 06 Jan 2023 19:02:44 GMT  
		Size: 5.0 MB (4978864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d0ffb9f3a02579d3758c82718e4b876091b11f2de18ac61f7ce002fad3f39b`  
		Last Modified: Fri, 06 Jan 2023 19:02:43 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddccb2d2cc74e2bd876b7b9c58e3a7dae1a93a978ad86e0cf016a3b268cf250`  
		Last Modified: Fri, 06 Jan 2023 19:02:42 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:c3f54742a5204c7905541fa75a98a4e3b4d935d1743fc86fafca8cb45c690ffa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7836628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:406197ad7c8143a2bc8fcf46e8f6c4e07fccb1ec56a5861635d08f3b36d5e66e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:06:27 GMT
ADD file:4696f25d0f019b27457c55b3b128b70bf153f38e3e4eb5bdfc21058543313e94 in / 
# Mon, 09 Jan 2023 17:06:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:42:55 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 17:42:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 17:42:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 17:42:59 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 17:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 17:42:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c527615e4ffa2d5b9b777fd469b3b5ba7c1b1e9201c065be2c43569de48a3754`  
		Last Modified: Mon, 09 Jan 2023 17:07:17 GMT  
		Size: 2.9 MB (2865208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d73a336145882faccd34809875f895c5656f01fecee5e507eb3f66921153ab`  
		Last Modified: Mon, 09 Jan 2023 17:44:08 GMT  
		Size: 5.0 MB (4970447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a17bb42266b7bab68da86f2509863bd7b0ef2ff9f7394264c43a21e372353c9`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1f1b4135d297a1a9a51450652100292d4907e3d8a675c5dea6b564a1d4b2`  
		Last Modified: Mon, 09 Jan 2023 17:44:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:9547980b254de3266558a6ef1df24731f1b81394580999af7f8e0f56ac535b5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8059465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:137eb6cff01cf8a79a84220b858e16f5d6bfcd5d49a33c2e1fb3a600d106ff0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:13:53 GMT
ENV NATS_SERVER=2.9.11
# Mon, 09 Jan 2023 18:13:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='0ff6e07f5cf211b643395132f63a69d69f0ed85ddcefd292b150574392e75edb' ;; 		armhf) natsArch='arm6'; sha256='d2c58d51c5050582ec1888107a6eea041745b287548a37e27569437a4725c3ed' ;; 		armv7) natsArch='arm7'; sha256='cef33d5b84473050e3dc0143117e336e90853e33d6329847612db88a1b8b139f' ;; 		x86_64) natsArch='amd64'; sha256='7491944084cd0128c1ddf9a313095817a2c558b0911581c98e65b84779110856' ;; 		x86) natsArch='386'; sha256='510eb4e4a32f1feba76232187767dd8ff0e021593f1cfbb6c5646343f3ca7a68' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Jan 2023 18:13:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Jan 2023 18:13:56 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Jan 2023 18:13:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:13:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5926ad44fb07bd1b6468b934276f66499dd403aaefc7e4a2425eecd6d1d6dee3`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 4.8 MB (4799229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee0a9e6a9ad8eabb0f8a9c119f5396c1e80a46027b3a389592c31355c7292fc`  
		Last Modified: Mon, 09 Jan 2023 18:14:25 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c2354f9e90a43e060a732dde40a2101e83a9a005c7bc393617a8b1fe1ee5a6`  
		Last Modified: Mon, 09 Jan 2023 18:14:24 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:3ba544a6bbef5767fb28be2737308833ea6f6fbddcb36cc0c8f42bef58ebaf33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3770; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:729dbc867ee0075d7a9a4ea3bf25f1f10116f3391578195299125f8e3a6c552c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:05e845fd1157584772ff668cf3c05e22f5616c6c30830ac25f3fd58918b93723
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111657318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b47fcb5910d5c05ee1f3c5949c04a43f04d50a36cbc06ef91e95b784cb3bd4f`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 02:41:38 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:19:53 GMT
RUN cmd /S /C #(nop) COPY file:a4a62c8491380467a4b102dd5a7b3261bb9b459208df8439f078271edc3f0844 in C:\nats-server.exe 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:56 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e9d361872b14736e9b1544993bd1f54f9284833fe47bff0ed4a51b726c47d8`  
		Last Modified: Wed, 14 Dec 2022 02:42:31 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5257b103d7abb48f945c26ecf455e90d3604c36c7d38e9ec9711f36d40a13a6f`  
		Last Modified: Fri, 06 Jan 2023 19:20:44 GMT  
		Size: 5.0 MB (4979867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f687f4813217f78031e69dde4d14441e507e48ac7e1ddf12b6ef7a459c77eb`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f04bf02165607b3e7d68f4764d8f440cdf86e58dd192654369fb196baaae8dd`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d3eca13a6e75fc248b139f92441d1dd434b973e7f8cd45f4c39fdaab97ad06`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92203cca3f700f40f1e2a46b108a0a51cd9f8542f7e0b8d82a45defb9f1bbe07`  
		Last Modified: Fri, 06 Jan 2023 19:20:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:ea67865b6a98fa17ea12f0daedb488cea79ec21909782099413e37f3eb4b5234
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:afeb1c1aab2036e50aa6224c94c689511caeeb550eed9ab9bb5858f4911f5503
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4926331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cc3017edab7b67e29f47c92b56cc34f0f8ebefa6fb8dc0d88c687289b768831`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:664b8b57454f3da8850d2d6ef93a053325e8bfd6ac97b3e7eb698f7ab97a8444 in /nats-server 
# Fri, 06 Jan 2023 19:20:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:20:20 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:20:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:20:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:20:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5508a75fcd75bf81905bd9dface9fc8d21aadf369f833d008d69b84105e348eb`  
		Last Modified: Fri, 06 Jan 2023 19:21:07 GMT  
		Size: 4.9 MB (4925823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eeb51c6bafbe9123bb07d5a7cce0ca930c05095f5a7e84bd8b18ce00ca863e`  
		Last Modified: Fri, 06 Jan 2023 19:21:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f99b07d5eeb8971c80cec3162acdac2900afbbfbef5dc64db1611b3e4fb13e10
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4690616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f5e7a92ad51faff09589ae0df91b06d2a55a2b4256f5f90eba2977ecf853a16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:06595cdf8db2d70bfb15c918efe6dd450e02ede2db1bb850d93a2a60bbf27df7 in /nats-server 
# Fri, 06 Jan 2023 19:01:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:01:45 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:01:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:01:45 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:873d4014d51427c81aca5b4db8b1b8a46b3d0815b34cdd333e34677aab4a7ba0`  
		Last Modified: Fri, 06 Jan 2023 19:03:15 GMT  
		Size: 4.7 MB (4690108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a283a79d5f31a899e117ab07ef87b81b7318fc27d705d7113398a1bfb28bb2a`  
		Last Modified: Fri, 06 Jan 2023 19:03:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:455074c66f1b96f45dbea5e8442f68edfb94af657dee605576061781047e582a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4685531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6a8534b65a22d58be02e8984744983e3c96c1f5e4c060dc057d23d8fec24bd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:5d6035836a154f215ce8e2c0418c0336bca5ac209aa8e275ca48920cc9b3f584 in /nats-server 
# Fri, 06 Jan 2023 19:15:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 19:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:15:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 19:15:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 19:15:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a2d610a1a25d4664f94b304a8a8f12e1d4f104226c5002b279d0499c3505a29c`  
		Last Modified: Fri, 06 Jan 2023 19:17:18 GMT  
		Size: 4.7 MB (4685021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbede3d18d47ba4e57885915c844dc259ebac29270369d6472059f4ab0e666`  
		Last Modified: Fri, 06 Jan 2023 19:17:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ffce0cb26fd6677a5ef05b45318360ae20e737bfdc2863d71bae13ec9bc5047b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4512312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f3692328c1caf31688888abde4f682928158ee544d2e3644095c9a2ecf9d16`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:19a72664362353bea19dae5d33666206cbba5c7e481270b1ebf62b792b7a49ea in /nats-server 
# Fri, 06 Jan 2023 21:38:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 06 Jan 2023 21:38:21 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 21:38:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 06 Jan 2023 21:38:21 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 06 Jan 2023 21:38:21 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4b1c65fa290503905ae36006eb2cd6d2df7267f54d65588f85ba20e700586ed6`  
		Last Modified: Fri, 06 Jan 2023 21:39:09 GMT  
		Size: 4.5 MB (4511804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256f83ce0dee80eadbf8b49697841b61fb25ace6c9a7682e596eb060a928836a`  
		Last Modified: Fri, 06 Jan 2023 21:39:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:5adb2736128fc9cdc9121921045732ceb89c29002bc1bfe018d6e948eb2b342f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull nats@sha256:4c98a74fa8012ed553add7c28d58950409b6c3c5c9b2e96bb9cd1d844a9a39ac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2786387516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b14b378c9702ccb1fa11eaebbe8ecb10e4528f7abcbd594a050a9a96fd03f5`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Wed, 14 Dec 2022 01:29:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Dec 2022 02:37:16 GMT
ENV NATS_DOCKERIZED=1
# Fri, 06 Jan 2023 19:16:03 GMT
ENV NATS_SERVER=2.9.11
# Fri, 06 Jan 2023 19:16:04 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.11/nats-server-v2.9.11-windows-amd64.zip
# Fri, 06 Jan 2023 19:16:05 GMT
ENV NATS_SERVER_SHASUM=f5cc4f7ca32dfe64f2bb35740cf824ddfae52b672c5e2775de3996f7beb6ff78
# Fri, 06 Jan 2023 19:17:35 GMT
RUN Set-PSDebug -Trace 2
# Fri, 06 Jan 2023 19:19:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 06 Jan 2023 19:19:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 06 Jan 2023 19:19:26 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Jan 2023 19:19:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 06 Jan 2023 19:19:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1d7d21a6f8359d8228f44b50aa9ad552783452100b6ce203e8f042415b5623`  
		Last Modified: Wed, 14 Dec 2022 02:14:22 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2b4fa0f968fba4be86c61da602c6d1d95bea2a5b257fa97e5cb498f7ddc7fe`  
		Last Modified: Wed, 14 Dec 2022 02:42:16 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb772b707da6af193f8cd8726ef6c899f782a6ff4d8db7294426432c311363c`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241ee848de8d88e39e2081b58c637a9f0c907f1107b1e87f752e9169e204a4b5`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173ec9d4380a9ae3a0bb21e0a218270752bc7c13b302e374cfc9cb34fcc83b8b`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25002b857471339cc5dd40dccdd55cd08b6946a05853407007f81a7d79b413ca`  
		Last Modified: Fri, 06 Jan 2023 19:20:29 GMT  
		Size: 358.0 KB (358013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61425272f47d38c91f87f342184e94d1b4f2a3188b2f5be4e1ca1c54bbcdb291`  
		Last Modified: Fri, 06 Jan 2023 19:20:28 GMT  
		Size: 5.3 MB (5319694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b89875960e791ac007a3c698c272b84c80f40b80429f92dccc0e718159af7f`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.9 KB (1868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17000f4b3f1a806bcf6fa2bd00063370bea6c4332161c0c3bba02b94d74fb1cd`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8859256765b04aecbba31a7d8aed786165846757d94059e22c0cdf79a0ab763`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9356faf9a606a778ebf57c726bf77aa3aa0bd527123f908d1178b3c9eb2db5`  
		Last Modified: Fri, 06 Jan 2023 19:20:27 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
