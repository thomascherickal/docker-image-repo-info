<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.13`](#nats2-alpine313)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.2`](#nats22)
-	[`nats:2.2-alpine`](#nats22-alpine)
-	[`nats:2.2-alpine3.13`](#nats22-alpine313)
-	[`nats:2.2-linux`](#nats22-linux)
-	[`nats:2.2-nanoserver`](#nats22-nanoserver)
-	[`nats:2.2-nanoserver-1809`](#nats22-nanoserver-1809)
-	[`nats:2.2-scratch`](#nats22-scratch)
-	[`nats:2.2-windowsservercore`](#nats22-windowsservercore)
-	[`nats:2.2-windowsservercore-1809`](#nats22-windowsservercore-1809)
-	[`nats:2.2-windowsservercore-ltsc2016`](#nats22-windowsservercore-ltsc2016)
-	[`nats:2.2.3`](#nats223)
-	[`nats:2.2.3-alpine`](#nats223-alpine)
-	[`nats:2.2.3-alpine3.13`](#nats223-alpine313)
-	[`nats:2.2.3-linux`](#nats223-linux)
-	[`nats:2.2.3-nanoserver`](#nats223-nanoserver)
-	[`nats:2.2.3-nanoserver-1809`](#nats223-nanoserver-1809)
-	[`nats:2.2.3-scratch`](#nats223-scratch)
-	[`nats:2.2.3-windowsservercore`](#nats223-windowsservercore)
-	[`nats:2.2.3-windowsservercore-1809`](#nats223-windowsservercore-1809)
-	[`nats:2.2.3-windowsservercore-ltsc2016`](#nats223-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.13`](#natsalpine313)
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
$ docker pull nats@sha256:00eb6d907368f5637e0ee0af3f0e1b8135b3bd4a87636d33ed1709201422cb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:95c7b2edb68fffeddc422d8b2a36778e3e589d9df49014991f4a2e9ea47134f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:28a61767d258d0e6d6d671831e1b24f3e0aac2c3a3d8893c42a962a8ad571692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:cae511104771f0231d31b8868ae3cac1b8f991bcb60e81b44733236d47525ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:00eb6d907368f5637e0ee0af3f0e1b8135b3bd4a87636d33ed1709201422cb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:95c7b2edb68fffeddc422d8b2a36778e3e589d9df49014991f4a2e9ea47134f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:28a61767d258d0e6d6d671831e1b24f3e0aac2c3a3d8893c42a962a8ad571692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:cae511104771f0231d31b8868ae3cac1b8f991bcb60e81b44733236d47525ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3`

```console
$ docker pull nats@sha256:00eb6d907368f5637e0ee0af3f0e1b8135b3bd4a87636d33ed1709201422cb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.3` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-alpine`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-alpine3.13`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.3-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-linux`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-nanoserver`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.3-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.3-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-scratch`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-windowsservercore`

```console
$ docker pull nats@sha256:95c7b2edb68fffeddc422d8b2a36778e3e589d9df49014991f4a2e9ea47134f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2.3-windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:28a61767d258d0e6d6d671831e1b24f3e0aac2c3a3d8893c42a962a8ad571692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:2.2.3-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:cae511104771f0231d31b8868ae3cac1b8f991bcb60e81b44733236d47525ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:2.2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:c767ab9d6eedf1a34936f3006a6b8f0d3f69ce8a6d42aacb7784b84886ff236d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:7918a8008609fff40bcf28275dd8d3379f3ebc8f24525b4787e6afd58272712b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7334107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b83664c1a0ab49aff75449d0d27ccc447e8c16ec7d9505e87f9224dba742d1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:20:09 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:20:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:20:12 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:20:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:20:12 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:20:12 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e986f351503b656bda4a2e07c65f7348c5a984498018311a0e615fe1e36fb22`  
		Last Modified: Sat, 08 May 2021 01:21:20 GMT  
		Size: 4.5 MB (4521168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acaa327c35c7298875823e2292cbb6ec9d6740dce8d7037693b0b0275e60a6f8`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbee1c4066c1f56267ac2a451ad9cfa9eca22989bbaf797ddd892cf682122567`  
		Last Modified: Sat, 08 May 2021 01:21:19 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:5c38980be68f2a66f391b3b8fc4943374b1263d1ad78ece87cafd58c9dac917e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6812948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af488973d954cc8e944c1062aa1efed650de8096695f600487483ae03e97c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:28 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:00:36 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:00:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:00:37 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae176648fd72c8ebc4f8ba3ec19886e9207de3a8ac11d74c7cae2ce253a3857`  
		Last Modified: Sat, 08 May 2021 01:05:55 GMT  
		Size: 4.2 MB (4189845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe80db509483996b6292319854a6c411144b29bea2d3e13affb25e8f940aa55`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47deb2430e024c01aecf98fe6bbb2f3b67367e1a8d2f1c735913811be016444`  
		Last Modified: Sat, 08 May 2021 01:05:54 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2eceda64ff33d418733bcb3066e2f9e37d90fd9249887c61a9a1d7045a0c996
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6611920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3acb00938c4c87cd4f58a03929151ce9dcaf80b3ee94d72836ec1f031ceecb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:00:50 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:00:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:00:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:00:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:01:01 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:01:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5b6437670afc66364f53d8e6f4ced4555fcc4675b5ead8d067c85bd837e179`  
		Last Modified: Sat, 08 May 2021 01:08:55 GMT  
		Size: 4.2 MB (4186801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f397b56e66d1e7e6c958171f69da3f8b024691f1671145a65cd6a94f29222749`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5513562bea4b2c543436df021533d03c9113fba5084ef89da05441814c075`  
		Last Modified: Sat, 08 May 2021 01:08:53 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ccc1fbfb4ac5164e84a03ff050cdbacf000ababc4fe4874925dc1b10bf31bc28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6874708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852b3a838a6aba2a9c7e01f85ec6598d55c3a828af0cd8bb1b7a5e1b6952fc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Sat, 08 May 2021 01:41:26 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6fc1c02eea8b376f9a2547b8129df1dccf2773490e4e3a85a743152d45dee4e0' ;; 		armhf) natsArch='arm6'; sha256='bc0d25a9e1cc37f3d859c135581b0ee2c6af6f86e0c1872e79a842d03ab6dd8c' ;; 		armv7) natsArch='arm7'; sha256='7d30205305a4ef20cc1b39894e9e7404058ff560cfd7ee90fc9b530a794b743a' ;; 		x86_64) natsArch='amd64'; sha256='818cf5079dc19d39bb22cf9f122ae5191f62d61619114c1b58ce00ba8a4e2517' ;; 		x86) natsArch='386'; sha256='81071f4c7ef5277cd29880cac2e0731de906ad1932fa2ce94641b455f2bb42f2' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 08 May 2021 01:41:32 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 08 May 2021 01:41:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 08 May 2021 01:41:34 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:41:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 May 2021 01:41:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db75540be659a546560457473da0f65381c03fab891f8d50109fbf069fa9522`  
		Last Modified: Sat, 08 May 2021 01:50:59 GMT  
		Size: 4.2 MB (4161711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694c713de077e6ef4060443ad7494444fae74d138f60c950000fb2e69dd15c1c`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65859d69470aa6901bf3eeb02e4433f62a0c6c98f68b2fc1eaa82f231465328d`  
		Last Modified: Sat, 08 May 2021 01:50:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:00eb6d907368f5637e0ee0af3f0e1b8135b3bd4a87636d33ed1709201422cb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:304c290d01432f65b23b8db072061924adf79790346cb65132a3c353fc30267f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:95c7b2edb68fffeddc422d8b2a36778e3e589d9df49014991f4a2e9ea47134f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64
	-	windows version 10.0.14393.4350; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:28a61767d258d0e6d6d671831e1b24f3e0aac2c3a3d8893c42a962a8ad571692
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:d7323469b7f3bf803d8db59cce7c9375b0c95627898b7ea51d364561b96ea174
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2484222239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce0ce6bf54d9a83dc699dc925cefc4da62be50613ad270dcd2d7cd2aed19e4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 13:10:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:02:50 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:14:10 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:14:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:14:12 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:14:43 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:15:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:15:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:15:57 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:15:58 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:15:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2159a5d0f75ce11e6fe71e4260ede5c3c88a9eb76a0ff43ac6746b2b9b96775`  
		Last Modified: Wed, 14 Apr 2021 15:37:10 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849354f21f856ec720d6daecc37978fd7246f376ba3c32fd63d4400cce357bc`  
		Last Modified: Wed, 14 Apr 2021 16:10:16 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a59546309673d4b20f6b764e6cdb66ef15109c8d058a3a6fafc152a44aad`  
		Last Modified: Sat, 08 May 2021 01:20:14 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c48747fca6c2cf91251deb0b3843f44b8758ebd29ee8fa0edce17b9f7dcfd5`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8193a715c0836417f1d9325ca56cd00c0108132642f3f0f22b98be9449c6b8d`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a6b950b0b7977911f8e95d23bfb1102309fd1c944f92fe940e056088742faa`  
		Last Modified: Sat, 08 May 2021 01:20:15 GMT  
		Size: 5.1 MB (5096312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da99923a0ffc9f03f1732f727ba585738acaab6860d0187a480de49558c2d9`  
		Last Modified: Sat, 08 May 2021 01:20:13 GMT  
		Size: 9.4 MB (9358928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28a1256dcb38b1bafce26f943536a7dd9a39c7ec54fd4136cc49a3f5ef6d8d6`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fab9f770e3ab4e0d968cb65264ae0e9bdd4382b8d3a70deb59617091b2af9a9`  
		Last Modified: Sat, 08 May 2021 01:20:11 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4f0c5e71e780eacc043bd6bd9aa62cee1de9e6fb4313c2b195a07f88757e5`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89f86179058b328103f74f4216154e7c83ad10dac41222649baf934a5ccacdc`  
		Last Modified: Sat, 08 May 2021 01:20:10 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:cae511104771f0231d31b8868ae3cac1b8f991bcb60e81b44733236d47525ab4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull nats@sha256:a601f0fba4299de34cb17a50c80f7dcdeb4100e139c8df4968d76b3de93cd7b7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814999141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0268ef7189c2659b5c9cf424c2237fab5ad356145b53400f1b936d0f8e6bee81`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 13:22:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Apr 2021 16:05:33 GMT
ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER=2.2.3
# Sat, 08 May 2021 01:16:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Sat, 08 May 2021 01:16:20 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Sat, 08 May 2021 01:17:30 GMT
RUN Set-PSDebug -Trace 2
# Sat, 08 May 2021 01:19:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Sat, 08 May 2021 01:19:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:19:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:19:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:19:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f616bb7876e6f944d82fa1802ffab5ca4931a63e1b999f0851b52120cda83539`  
		Last Modified: Wed, 14 Apr 2021 15:37:43 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfa54f43457753c391f21da5e9a5bf47c61c574c0da04b8614d0e84bf823f54`  
		Last Modified: Wed, 14 Apr 2021 16:11:03 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd73175def227cecab8b1d0daabaed653bf698b3998df811f26df3e7e33b9c2d`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0d0372510261d94e492fc4b8c34dafc5312b85ed72685a2856304eee289a3`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203b90b72277f99d3111385c98ebdb1e34e0515ec30a8d6eed17caef4e21cbcc`  
		Last Modified: Sat, 08 May 2021 01:20:50 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cadf6fcab56a60838248eb1f6b2ac2273141b7a404a2ab9e0c0d89f9f9d94b`  
		Last Modified: Sat, 08 May 2021 01:20:52 GMT  
		Size: 5.7 MB (5653916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2609d85a6e72ac850af35a809109dde27760e08c3f1a1916e1b35b51aa821047`  
		Last Modified: Sat, 08 May 2021 01:20:51 GMT  
		Size: 14.4 MB (14448135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6c38534554dbb86ddeacf527c41ce516c03d8847dba5b0dc30f1f4d23b51fe`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0791626a30dce3a517c9e41798b4874a9b6419ebde4d059b8abb16c4021e7e`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e367eb9da2f71bab653cf5676c106509a942bd9f2a907f9cca1f447e3e8d6be`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a90a989e400a5782487b7cf7d4ec14cc1593da49ee757bbb502ca5769131c32`  
		Last Modified: Sat, 08 May 2021 01:20:48 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
