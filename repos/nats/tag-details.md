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
$ docker pull nats@sha256:bd6a4627682764497ea74e910a47ada6aa5a794136b5fae097fa676262a81edf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

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

### `nats:2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:450bcbcdd85897b9a7a28a99d34701450223b7b96b39838e95493abd18e77829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:92af18909a07b17d44c1b4dab108c3ec79f738445924832589a1f038531f9aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b54ef6b58efd31523be8c864e843428ca2d8976ce534b058079a389666f4fa90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:bd6a4627682764497ea74e910a47ada6aa5a794136b5fae097fa676262a81edf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

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

### `nats:2.2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:450bcbcdd85897b9a7a28a99d34701450223b7b96b39838e95493abd18e77829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:92af18909a07b17d44c1b4dab108c3ec79f738445924832589a1f038531f9aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b54ef6b58efd31523be8c864e843428ca2d8976ce534b058079a389666f4fa90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3`

```console
$ docker pull nats@sha256:bd6a4627682764497ea74e910a47ada6aa5a794136b5fae097fa676262a81edf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

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

### `nats:2.2.3` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.3-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.3-nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:450bcbcdd85897b9a7a28a99d34701450223b7b96b39838e95493abd18e77829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.3-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.3-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:92af18909a07b17d44c1b4dab108c3ec79f738445924832589a1f038531f9aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:2.2.3-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b54ef6b58efd31523be8c864e843428ca2d8976ce534b058079a389666f4fa90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:2.2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
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
$ docker pull nats@sha256:bd6a4627682764497ea74e910a47ada6aa5a794136b5fae097fa676262a81edf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1935; amd64

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

### `nats:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:63cbe4e8a745d068f30d1fc757f589ee984384dba70a21b06e599a3c503f3749
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:567e0ff61eb0a65c91223af7d082535ef6d531b9642e53e22193341e5711b6d9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105675980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69b53cab6e8045ed44c49a74fe549e74731a88c246b5e56ac756b62e6bfae6d7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:04 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Wed, 12 May 2021 15:44:05 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:44:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:44:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:44:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e22b5d6310eb052787cad7bd9f860153e1873fa68423ccba39726c63bb41f2`  
		Last Modified: Wed, 12 May 2021 15:49:04 GMT  
		Size: 4.3 MB (4294368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7f45222cce584a936e09af045a2a179963bfd6f23566f42b8201c9f8531101`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfe82cf96b4d08f2bb9baaf769eb0c66a75ec3ce19e774825fc888990942f8c`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cfde2dbdc484f782e2189f69d548a80fe02d0680a7b14856ba6548f8a4d518`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd177c2329a35a15fbb6add029d14b3584ccaf702d13eefd211958ec39e1fce7`  
		Last Modified: Wed, 12 May 2021 15:48:59 GMT  
		Size: 1.2 KB (1151 bytes)  
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
$ docker pull nats@sha256:450bcbcdd85897b9a7a28a99d34701450223b7b96b39838e95493abd18e77829
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:92af18909a07b17d44c1b4dab108c3ec79f738445924832589a1f038531f9aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats@sha256:b8f78fa18e95ccd030921491099bdde6027366e20ac29724826806ccc57a8fc0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2488959507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b8a5009e27b5f8b20992ed668c1df65a85d913c82c98d32438569b82c04a87`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Tue, 11 May 2021 23:54:13 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:41:49 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:41:50 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:41:51 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:41:52 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:42:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:43:40 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:43:42 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:43:43 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c049a65ed9206719f5c04428cb853623400e8ab1668243872b1134775f752962`  
		Last Modified: Wed, 12 May 2021 00:41:58 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d2305f11fe8f36ef3508b42686daac7e99da966ed02f4ded1927387b1b75b`  
		Last Modified: Wed, 12 May 2021 15:48:42 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997292a293a04bf9999ffa301783c44d32ec86576fc6e0a67f833d0e3681d31`  
		Last Modified: Wed, 12 May 2021 15:48:39 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e994dfe884b3f7ba067e339ef8c984b37b3b677863aa953ad40d3bf4b74536`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c068dad32902ef5213f961601255c3f502986f4a52c117ce6ee6a29c14748b8a`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536fa26cb9cd7685db7d4789aeeb434b2d4429f94e1b149374cc64d27a07e5bf`  
		Last Modified: Wed, 12 May 2021 15:48:40 GMT  
		Size: 5.1 MB (5096854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882208c7ca121b0cd4752cf236a1b481d05c046c612f9674b1602c1d665d88ba`  
		Last Modified: Wed, 12 May 2021 15:48:38 GMT  
		Size: 9.4 MB (9360268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f1a7d478f8c7670b3917c6c5518713e8b3639b3bc7bded3a99a5543c1f63fe`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.9 KB (1940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e39ab211e123a59eca138ecb7270eb494cf5fcd3a62952bbb56475be5c1b747`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced6934e21457558d4cc707f30d7e4a0fe02679a0cb4318e0290f20f32d95942`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bd6d132abe90d38c813e09d681d04097ef025ecb6a1da311c882bb7db84ea`  
		Last Modified: Wed, 12 May 2021 15:48:36 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:b54ef6b58efd31523be8c864e843428ca2d8976ce534b058079a389666f4fa90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull nats@sha256:a1afdd3ea8f102dcc62a70bfb082588bc4b184becad2469e752c8e126ab6df53
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815946596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b825a3f2e49865904aba44cc6f5a2c8b80c0189b1c372477e32ad2c3545888`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 May 2021 23:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 May 2021 15:44:16 GMT
ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 15:44:17 GMT
ENV NATS_SERVER=2.2.3
# Wed, 12 May 2021 15:44:18 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.3/nats-server-v2.2.3-windows-amd64.zip
# Wed, 12 May 2021 15:44:19 GMT
ENV GIT_DOWNLOAD_SHA256=7f1ad2f52a6983b2ef9a1bf909ecebe2d0d3c3f5a84b84dacc63bf7fd8948c46
# Wed, 12 May 2021 15:45:40 GMT
RUN Set-PSDebug -Trace 2
# Wed, 12 May 2021 15:47:49 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 12 May 2021 15:47:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 12 May 2021 15:47:51 GMT
EXPOSE 4222 6222 8222
# Wed, 12 May 2021 15:47:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 12 May 2021 15:47:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:50d0f4595a2bdc5dc0623fbee162be09d0631373eb9e82a0b1ec387ce1512c49`  
		Last Modified: Wed, 12 May 2021 00:46:32 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7998d92dbbcfc4e6dc106e75206a3cfde70fe601eb46b0515658f23dcd53ae`  
		Last Modified: Wed, 12 May 2021 15:49:26 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6646c0a4909dd219ffb3eb6eb3709b768fde40ba969a0416a73716211f2a2ef1`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d117e0e9fd386f6d4c004ecf8c18fe24981e5dcf7396ba7935598c16d63d2e24`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c98fa15ec3d078cc3f3da05a4adc67ef14ad1abad5f9e06af54f26121a1d298`  
		Last Modified: Wed, 12 May 2021 15:49:23 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac43c7bec6bd3c410f67cd8fc3336f2ff913251c6251c48f877908df661c8ab3`  
		Last Modified: Wed, 12 May 2021 15:49:25 GMT  
		Size: 5.7 MB (5705594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af8fbf17e86d247bfd4abf90eca1d1e8682d466716786f01230a300844d893f`  
		Last Modified: Wed, 12 May 2021 15:49:24 GMT  
		Size: 14.5 MB (14450465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236726b5e955bfd7dd64337c1e1f23a903cfa204639b0a377b13f86297815f66`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231f23209351216b06233ad4059b5a5e3eef3e3f5d38896f2306d69bca7efa56`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64daeb968b2f9ad52152de233e969ab4a7acbd81b939b6d12ce9476c61284b7`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6af4f8b0031c6ff433713d50b0f460a68c589538710d23ff6b592b4b1e575e`  
		Last Modified: Wed, 12 May 2021 15:49:20 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
