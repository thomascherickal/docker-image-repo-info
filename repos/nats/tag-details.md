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
-	[`nats:2.6.2`](#nats262)
-	[`nats:2.6.2-alpine`](#nats262-alpine)
-	[`nats:2.6.2-alpine3.14`](#nats262-alpine314)
-	[`nats:2.6.2-linux`](#nats262-linux)
-	[`nats:2.6.2-nanoserver`](#nats262-nanoserver)
-	[`nats:2.6.2-nanoserver-1809`](#nats262-nanoserver-1809)
-	[`nats:2.6.2-scratch`](#nats262-scratch)
-	[`nats:2.6.2-windowsservercore`](#nats262-windowsservercore)
-	[`nats:2.6.2-windowsservercore-1809`](#nats262-windowsservercore-1809)
-	[`nats:2.6.2-windowsservercore-ltsc2016`](#nats262-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:7a014b4f0b3f00c1942a7c5cc6087f2683eae9571cf63f86e6580de55f761a3f
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
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f182ccba53852c99b1d513a23e83b7c4ac54c4130240845ebf197adc3327c1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a6c76e3e7ee7ecbf036ee26145711375e8543998dc1512413e108477dbd310f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ca9cf9ebe4d0aa6306e7b53a7a092ccd2f69eeec24646357a0eef697bdb4f647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6`

```console
$ docker pull nats@sha256:7a014b4f0b3f00c1942a7c5cc6087f2683eae9571cf63f86e6580de55f761a3f
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
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine3.14`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-linux`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-scratch`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore`

```console
$ docker pull nats@sha256:f182ccba53852c99b1d513a23e83b7c4ac54c4130240845ebf197adc3327c1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:a6c76e3e7ee7ecbf036ee26145711375e8543998dc1512413e108477dbd310f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ca9cf9ebe4d0aa6306e7b53a7a092ccd2f69eeec24646357a0eef697bdb4f647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2`

```console
$ docker pull nats@sha256:3167fa2c67cb235672992c81f47ccec454a2ec404374a8b23dc69225b41cdf63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.2` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-alpine`

```console
$ docker pull nats@sha256:464eb8c9f567564e906916dee106b871ad331d9d88d8e68fb7f92abe8190bda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.6.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-alpine3.14`

```console
$ docker pull nats@sha256:464eb8c9f567564e906916dee106b871ad331d9d88d8e68fb7f92abe8190bda3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.6.2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-linux`

```console
$ docker pull nats@sha256:be76b3f567bd06cc1db8c5b15a1d59faf9c44307463c85253e56c800ee391291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.6.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-nanoserver`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.2-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-nanoserver-1809`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.2-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-scratch`

```console
$ docker pull nats@sha256:be76b3f567bd06cc1db8c5b15a1d59faf9c44307463c85253e56c800ee391291
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `nats:2.6.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-windowsservercore`

```console
$ docker pull nats@sha256:f182ccba53852c99b1d513a23e83b7c4ac54c4130240845ebf197adc3327c1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.2-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.2-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a6c76e3e7ee7ecbf036ee26145711375e8543998dc1512413e108477dbd310f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2.6.2-windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ca9cf9ebe4d0aa6306e7b53a7a092ccd2f69eeec24646357a0eef697bdb4f647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:2.6.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:8ffeb310d3ca33f5c5cad8f2a1cb6f971ddfc3fa264c05f46daa26cc09190eb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:14cc6a656f138d1e3e707e88c18ef88452b29ccb72af4176b8f5f78d23748030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7655041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5d1cad0ce15a4e94e87f82b966b73e25ba0d4629eb29c09178beb3f5af0b43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 18:20:14 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 18:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 18:20:18 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 18:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb318bc128d118ab570ff784f370b12bba9799d4b8ead06996ddb459d55ba9f4`  
		Last Modified: Fri, 24 Sep 2021 18:21:22 GMT  
		Size: 4.8 MB (4839621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abea9d20040e530947975d310bc6504f29c3518f07ca9320cf04a81b0372d03`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 561.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f787462ffd44dbb2ccc478572962380ecf84219b3f54034a8244cab789596707`  
		Last Modified: Fri, 24 Sep 2021 18:21:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:b66e17fed81f78bfbade4b7df09380660a6116411d67d0f35c45bc9052371006
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7137044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f19d7e07b4a0f3fa0b0ba0130868922801363e4bde23047bbc98550870e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Oct 2021 23:49:34 GMT
ENV NATS_SERVER=2.6.2
# Tue, 12 Oct 2021 23:49:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='040b4fbd896240d91dfec258d159731fa98eac0a8329a0009c65dee8a875d1a0' ;; 		armhf) natsArch='arm6'; sha256='1bba8a38b61bc4f95bc89a4038b34c7dadbd5e05ca93e4a28d0b98cc11b1c101' ;; 		armv7) natsArch='arm7'; sha256='ef0a719476e5e84f173c7abcf379c7a2ae8b1472ad397fd9e72909362f426679' ;; 		x86_64) natsArch='amd64'; sha256='cc6c6b737e8ecadbba2480518897c5a9fd2168fdd8115664a734f582d4c8c759' ;; 		x86) natsArch='386'; sha256='785539ec342ca08ebbfff72871ec570b19c3eee29dc357c0047af33aa387dadb' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 12 Oct 2021 23:49:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 12 Oct 2021 23:49:40 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 12 Oct 2021 23:49:40 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:49:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 23:49:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dac4814d8a10e132980bc0c9fc26f1b132815155952b39410b19de4bdfffb`  
		Last Modified: Tue, 12 Oct 2021 23:51:48 GMT  
		Size: 4.5 MB (4508626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc1ac7d223637b9928337142770c52955d5340766ff58dcf405505f154442eb`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ddd7eaa459a35633b8f07a40f5f36fa5f9666c49347b9341a0ca30f502dbb3`  
		Last Modified: Tue, 12 Oct 2021 23:51:45 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:d9fc63779407554a8674633e5732621f680292866c780da9f007ce29d75542e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6927152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e1c6d9848dce815735e333708e9e35533486997ca7f3031b655d4c398a92b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Thu, 30 Sep 2021 19:47:23 GMT
ENV NATS_SERVER=2.6.1
# Thu, 30 Sep 2021 19:47:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 30 Sep 2021 19:47:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 30 Sep 2021 19:47:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 30 Sep 2021 19:47:29 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 19:47:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00126b6dca785aa0a1a05eae3f9dca609d9677a0b164c6f686ab687589b5a3a`  
		Last Modified: Thu, 30 Sep 2021 19:49:42 GMT  
		Size: 4.5 MB (4495760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fb5271d804ff6a23c62bea2d0df5fe9b68466315efe98ab09239efa418c9`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47f9daa3ced3fd472321b155a7206875a5603a287f70b05bdd184ffbd55c647`  
		Last Modified: Thu, 30 Sep 2021 19:49:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:38888e1c67f76b7edbb92804a050b5de8e4e4f6ae8a980f919d17de7f1fcd4f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7162092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:700188dc91cf1626d6b15bb088a273301826130510c19b4dcc9fa42a7f8592ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:40:05 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:40:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:40:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:40:08 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:40:09 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1047b8662a09fdfa7dea8086cf9e2a632d09dd8f2848de9a500d15ae3c2bf7a9`  
		Last Modified: Fri, 24 Sep 2021 17:41:28 GMT  
		Size: 4.4 MB (4449294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84477e5068504078a4d643a66ae31db7aead8076162df1016404ea7f6ec479f9`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c94a831ef4c3b67a6834a3a36c58f4d6c60d52de703d7780d6d7ef071673bd`  
		Last Modified: Fri, 24 Sep 2021 17:41:27 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:7a014b4f0b3f00c1942a7c5cc6087f2683eae9571cf63f86e6580de55f761a3f
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
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:9dfe282350d007004b868fb9d3285238f6f805738c4683e1b4389e0a42d20876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:323758984f7ff928f2ee4e1edbfcde0c627e5e3251da3ab3b0c5e1b904a865d6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107287270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523b7f4d0c35a61dcd048c7d40753106abb7db8f18ddfbff2881a0fec9bb6e42`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Oct 2021 00:39:11 GMT
RUN cmd /S /C #(nop) COPY file:a277a9f60e868548242fc63bee0b041e8e60599cee831619883e36cef7abcc5c in C:\nats-server.exe 
# Wed, 13 Oct 2021 00:39:12 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:39:13 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:39:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:39:15 GMT
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
	-	`sha256:240ef18c46fea26f7a314bff9fe9bebb6cdf1a9ce5c88f2388e0b6e439443f1c`  
		Last Modified: Wed, 13 Oct 2021 00:43:57 GMT  
		Size: 4.6 MB (4619534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0917309333ff9845a654d19e7d7f7f388fe9fd380abca7cd7908f39fc63e5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a63ed99b3269c9dff06d460f8572688093b93789b641407811461c63e2ab4d5`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f0ff1500ee68b5adbb43f5e00141bde3ffd2670af0fc3f8f393aa4a5db13a0`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19972b0511610d0cd224fcd7de906126220b060d9980902fd67bedce45bf3fcd`  
		Last Modified: Wed, 13 Oct 2021 00:43:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:3fc750893be98b2000d3dfce4ecebf6f93e64db1d0d6bfdf205420132f3fc28c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:a43c679fb63f49a56f6710d3f4afaef53226518d9433f814f60ce9ea52b7799e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4557856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a38932d62612b28ddaad81d77d2a01622145f4361d28295cec7f6987c2511d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:56cc63952bfc4b2de2d1c200fd8cbf8f038a5f5f11289a52868a5df2375492b0 in /nats-server 
# Fri, 24 Sep 2021 18:20:54 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 18:20:54 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:20:54 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 18:20:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d16cac695b49a91619219e07a1503c4b96bcbe05f6b920081821c5efd29327e2`  
		Last Modified: Fri, 24 Sep 2021 18:21:47 GMT  
		Size: 4.6 MB (4557381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c945b005f9f3d8bf10851073ef8acbc52c6f2684a073d4068fc6d5b4e5848334`  
		Last Modified: Fri, 24 Sep 2021 18:21:46 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:93693c23ea5644f401a72bf6929214e9dfd2720b1b4c373025e689c1495de5a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4228700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1d37c768b08a19ab2b56aff52bc2bd23a18c665a38568b80d03d43b91ebe1d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 12 Oct 2021 23:50:02 GMT
COPY file:87c492688776372ccf80f66cfc3e90fd8fab44035811506c7aaa232e547e000b in /nats-server 
# Tue, 12 Oct 2021 23:50:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 12 Oct 2021 23:50:03 GMT
EXPOSE 4222 6222 8222
# Tue, 12 Oct 2021 23:50:04 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 12 Oct 2021 23:50:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3cd12bdf7a9a23f7457d02e8fc11f170382a386c0eeca79fe881fb322825f1a9`  
		Last Modified: Tue, 12 Oct 2021 23:52:26 GMT  
		Size: 4.2 MB (4228225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d6a7556bfb5d88c2ff5e698fcd012e06a282a35550cc4944de84fe772a4481`  
		Last Modified: Tue, 12 Oct 2021 23:52:23 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d2e70b8a1a863ae0f789502434cef995627ed0f46f551f291f2f7a0ff7017642
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4213288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3787a15077edfb6d8fa1646ed439c24cc005849fcf8311a629d20c8679d8b139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:6d69eef0d821da908da152f3dfe853b07d173db35f1c40a85e545d8218aaeb7e in /nats-server 
# Thu, 30 Sep 2021 19:47:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 30 Sep 2021 19:47:58 GMT
EXPOSE 4222 6222 8222
# Thu, 30 Sep 2021 19:47:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 30 Sep 2021 19:47:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c67bb3b32b6353245cbd27e1ee30c47b5cf8b7c76346ca37875fa7cc7086cf7e`  
		Last Modified: Thu, 30 Sep 2021 19:50:22 GMT  
		Size: 4.2 MB (4212814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065d109fdaff0adc51732a8f449fee6ffda396a8e2a53cda9273482aa1fb36f0`  
		Last Modified: Thu, 30 Sep 2021 19:50:19 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:2475df2d82899c998486ff164f63c549ab94f3ec9d6b6ced5f1a828feb097cbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd70c0c61ec57441666601ccff002d189c00d3ecb3a1eb1ea97f052736bee1b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:40:34 GMT
COPY file:9b757ffadeb4943a3ca6c78d9caf65891c08587f5bebf5be32974d1456afb89e in /nats-server 
# Fri, 24 Sep 2021 17:40:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:40:35 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:40:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:40:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7d0e0caa3737fe1355285d221e0c8e078337a45e1506022ffc37197d044d1db3`  
		Last Modified: Fri, 24 Sep 2021 17:41:58 GMT  
		Size: 4.2 MB (4169531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f509df5c28970b2ba96c7084c68158896b7fcbf5faf2d170a8d8e61960294c8`  
		Last Modified: Fri, 24 Sep 2021 17:41:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:f182ccba53852c99b1d513a23e83b7c4ac54c4130240845ebf197adc3327c1f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a6c76e3e7ee7ecbf036ee26145711375e8543998dc1512413e108477dbd310f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:8ff35373832a1c26ed5d2436fa9ed8175e522a319b6ebef541edd39ea0a0f1b2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691630742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c14d051353dd99010eae8c9f9718f52f79602895668613a54d2314aef1e487`
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
# Wed, 13 Oct 2021 00:34:12 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:34:13 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:34:14 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:36:25 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:38:50 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:38:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:38:52 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:38:54 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:38:54 GMT
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
	-	`sha256:24a473912d23203344681a1a41d78c25e7db4d53f09f158b9324e5cfbecdc036`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e1846d6e4fe0e87e2df499c3aeaf33ad463a1ad771712d959cf4eae67afcb1`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729a5ee4eb0be598f7b4892b34e36fb08ff7af94a9f3afd604a4d7c1820710d9`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c319f94bf8a8ecad2adef4af424689f9e02f9a67f6c7f81a6858e74ffa856e27`  
		Last Modified: Wed, 13 Oct 2021 00:43:38 GMT  
		Size: 343.5 KB (343480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3760335e1e38731733fe55c481c040d46a63f09f8b88145b6166b0158377367`  
		Last Modified: Wed, 13 Oct 2021 00:43:41 GMT  
		Size: 5.0 MB (4955632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5d153a47c11aa74fc78b9f5639dc086c9507c17e7870810816525b79ba2f7e`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 2.0 KB (1975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1150ca3565dd7cee47e86c6b10381c5458783ff399b1741dfcc7b161f6c983`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315796d10776e00340d0be3d6a09ffebcb6567372088686b64a26820197b8307`  
		Last Modified: Wed, 13 Oct 2021 00:43:35 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93008d6d2a7cc3a73e2b56b0a7a76fd86dd2d4b6cf0320ef9e52ed5031d815a`  
		Last Modified: Wed, 13 Oct 2021 00:43:36 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:ca9cf9ebe4d0aa6306e7b53a7a092ccd2f69eeec24646357a0eef697bdb4f647
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull nats@sha256:418f75da35917511a99273b446dfdd3b9af8ebe30c5d426238b560732cf34164
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278098651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ff3a0c76070dc9acbd5f90fc2a782f7a6961f87a2133c161ccb245055dab40`
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
# Wed, 13 Oct 2021 00:39:26 GMT
ENV NATS_SERVER=2.6.2
# Wed, 13 Oct 2021 00:39:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.2/nats-server-v2.6.2-windows-amd64.zip
# Wed, 13 Oct 2021 00:39:29 GMT
ENV NATS_SERVER_SHASUM=eb809cd5d2cd74edac1b3b770fdd09f9d98a970e14b24b0c2b5e4a8c538693db
# Wed, 13 Oct 2021 00:40:55 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Oct 2021 00:42:48 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Oct 2021 00:42:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 13 Oct 2021 00:42:50 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Oct 2021 00:42:51 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Oct 2021 00:42:52 GMT
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
	-	`sha256:594cc3f90d80a96c00df55188626147f8170f580b7a712a0c1a975dc380810a4`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9c3734400dd553e993f978090779922711884084c6b9a08af8a80c2a4c03d8`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5512210ab9d2dd13dbf25ad44b0abbe94f44ecc69232accf2bb4f33b4374fdb`  
		Last Modified: Wed, 13 Oct 2021 00:44:13 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c468f554d337e3a687604929a6519c0c88de7093c175ab49843c390c084c48`  
		Last Modified: Wed, 13 Oct 2021 00:44:14 GMT  
		Size: 340.2 KB (340186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f40948c5a62dbd876eb1e51cb91daa60ca1c32b8b38708df7f00db35c72d7ba`  
		Last Modified: Wed, 13 Oct 2021 00:44:17 GMT  
		Size: 5.0 MB (4978594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b76e0e528c691436c7e1006a94cd748a73b32eea4003cef86de73ae3516b30b`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aa08fc51be79a24b847a81556633117e27175161b1f614adaaff26405db431`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.5 KB (1452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570aa2e9cdad8f81f73820da764a7820ed0a28d7100d87f742322ba78d90f05a`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc825431ed33b4460730dbd1909422da70adbffeaa8f8586711474f5780d733e`  
		Last Modified: Wed, 13 Oct 2021 00:44:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
