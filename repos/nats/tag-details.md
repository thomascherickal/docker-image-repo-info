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
-	[`nats:2.6.1`](#nats261)
-	[`nats:2.6.1-alpine`](#nats261-alpine)
-	[`nats:2.6.1-alpine3.14`](#nats261-alpine314)
-	[`nats:2.6.1-linux`](#nats261-linux)
-	[`nats:2.6.1-nanoserver`](#nats261-nanoserver)
-	[`nats:2.6.1-nanoserver-1809`](#nats261-nanoserver-1809)
-	[`nats:2.6.1-scratch`](#nats261-scratch)
-	[`nats:2.6.1-windowsservercore`](#nats261-windowsservercore)
-	[`nats:2.6.1-windowsservercore-1809`](#nats261-windowsservercore-1809)
-	[`nats:2.6.1-windowsservercore-ltsc2016`](#nats261-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:a3d65d25c1c64911c9686e6cbf96ea8e2dd0763beb3906f6716d5e0da896367e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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

### `nats:2` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:599a1dfd68ec271f0feb5380fc72a4ba9866c30c7f1d36dc4830ff7ec374de73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:5378bb9ab24c93ab0346dfaf7cd89a842513cb88c8f44680cb3e5045c085ddb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:75e4ff61015f3bf7c22351ff65fa904e8d4dc1323aa7f8881dfa10a7c2ffa49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6`

```console
$ docker pull nats@sha256:a3d65d25c1c64911c9686e6cbf96ea8e2dd0763beb3906f6716d5e0da896367e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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

### `nats:2.6` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-alpine`

```console
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-nanoserver-1809`

```console
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-scratch`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:599a1dfd68ec271f0feb5380fc72a4ba9866c30c7f1d36dc4830ff7ec374de73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats:2.6-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:5378bb9ab24c93ab0346dfaf7cd89a842513cb88c8f44680cb3e5045c085ddb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:75e4ff61015f3bf7c22351ff65fa904e8d4dc1323aa7f8881dfa10a7c2ffa49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats:2.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1`

```console
$ docker pull nats@sha256:a3d65d25c1c64911c9686e6cbf96ea8e2dd0763beb3906f6716d5e0da896367e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6.1` - linux; amd64

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

### `nats:2.6.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1` - linux; arm variant v7

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

### `nats:2.6.1` - linux; arm64 variant v8

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

### `nats:2.6.1` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1-alpine`

```console
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.1-alpine` - linux; amd64

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

### `nats:2.6.1-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1-alpine` - linux; arm variant v7

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

### `nats:2.6.1-alpine` - linux; arm64 variant v8

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

## `nats:2.6.1-alpine3.14`

```console
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.1-alpine3.14` - linux; amd64

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

### `nats:2.6.1-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1-alpine3.14` - linux; arm variant v7

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

### `nats:2.6.1-alpine3.14` - linux; arm64 variant v8

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

## `nats:2.6.1-linux`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.1-linux` - linux; amd64

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

### `nats:2.6.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1-linux` - linux; arm variant v7

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

### `nats:2.6.1-linux` - linux; arm64 variant v8

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

## `nats:2.6.1-nanoserver`

```console
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6.1-nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1-nanoserver-1809`

```console
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6.1-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1-scratch`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.6.1-scratch` - linux; amd64

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

### `nats:2.6.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1-scratch` - linux; arm variant v7

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

### `nats:2.6.1-scratch` - linux; arm64 variant v8

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

## `nats:2.6.1-windowsservercore`

```console
$ docker pull nats@sha256:599a1dfd68ec271f0feb5380fc72a4ba9866c30c7f1d36dc4830ff7ec374de73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats:2.6.1-windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.6.1-windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:5378bb9ab24c93ab0346dfaf7cd89a842513cb88c8f44680cb3e5045c085ddb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:2.6.1-windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.6.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:75e4ff61015f3bf7c22351ff65fa904e8d4dc1323aa7f8881dfa10a7c2ffa49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats:2.6.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:e1dd4da2dd3f87d48ee4c83060d576688b65def12de6eb8f43a85fc7d694795f
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
$ docker pull nats@sha256:a1a401c2dd42ed8081e7ebf328dd7f9dd6ffe9dad928bd908a2dc7a0961660a0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:128ff61bfd32f451b68421543236d227440c88041c46314a65b7b3604efcc7ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 24 Sep 2021 17:49:42 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 17:49:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4354bdc411f63fa1528479b39b9312de1e1c23531136d88c6b58978dcbf1ec29' ;; 		armhf) natsArch='arm6'; sha256='65473af9ff2f0c75b65609722ad8eb37ee495b382a16697b0168a02abd7bf0f9' ;; 		armv7) natsArch='arm7'; sha256='c95287f62472566bbe30941b57dc4df6547ea5d6219615c3666ae4d5f3acd9d9' ;; 		x86_64) natsArch='amd64'; sha256='9168ba515d68cce426874096d0be2510d9846de66c74c7ab3ecbdc2a27e9c114' ;; 		x86) natsArch='386'; sha256='8f83456101181c7a0a59e83be03c4ec54d6a34737609d97575e2a4f47a08aa24' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 24 Sep 2021 17:49:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 24 Sep 2021 17:49:49 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:49:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Sep 2021 17:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93c29b9a608654f6f3250d956bd76a6258cd040dcce775e03f76f69b935124`  
		Last Modified: Fri, 24 Sep 2021 17:51:54 GMT  
		Size: 4.5 MB (4502338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07b9b15d4e0d0c308fad89b3cdac4e3ec483cfb76b99d9ebaef8467df2b9044`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ebd3f91acd6d1cb72a6ba50ed3b318d260069adbecd9a3b828c6d1ab0f66db`  
		Last Modified: Fri, 24 Sep 2021 17:51:51 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:a3d65d25c1c64911c9686e6cbf96ea8e2dd0763beb3906f6716d5e0da896367e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64

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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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

### `nats:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:nanoserver` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:6130f3021a163a22b1f0ba256bb2699c9a4ed30369086c8a4fccff5544206cd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:71c153413bf49b38806c3ad0c2a85c117380534d5d8587c9e930ad7061197323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107323878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8917f61d9feda334e63e3bb8a7406359fccecff0aacc392edaf7b993af8e1f33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 15:43:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:25 GMT
RUN cmd /S /C #(nop) COPY file:e8e5cb48daba80f34796952e26cc4058ca5809e456780e196277b4f6b98248b9 in C:\nats-server.exe 
# Fri, 24 Sep 2021 18:18:26 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:27 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:28 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66dbf96361e9ec1f64f66e255a947eab476edef46c3f9a3b4ede943fa8b87699`  
		Last Modified: Wed, 15 Sep 2021 15:46:11 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a89e42bde9eba1e3c234a1b0fa3c923f6980959a141c870e6d8b49353b89c52`  
		Last Modified: Fri, 24 Sep 2021 18:22:59 GMT  
		Size: 4.6 MB (4613776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71520d14dc0a4fa2ff138a03b2e1cba90e07a07e5d8a4095bf4939e740ecb4`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd964bd5c073449877455885b3d3466daa9f611ce0979ea4c4fd13f8d586721`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f529e09f796786e8eefc1792f39c3dcad6a7fb167fa5ead20c40310f632810`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a619e9f3c2ad169084d8726e34725b9a6f47e3a0cbc88a2433a04b76b32e23`  
		Last Modified: Fri, 24 Sep 2021 18:22:54 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:5299ba7db60603ffc7b4817d703652013010de656e2d934447acf13ef4c4bd83
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
$ docker pull nats@sha256:e118369f9d934b1ec7448fbe338ace258cc5804eac4139d730a5e38d0a34c27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4220173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03b6288e241bc310a2054420f7116dd72723916c9b1d55d401c281862cd899ae`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 24 Sep 2021 17:50:10 GMT
COPY file:2868e45519ac86c84fbede972aaa567adf799b1102fddd7627fd1a1ef86df5cc in /nats-server 
# Fri, 24 Sep 2021 17:50:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 24 Sep 2021 17:50:11 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 17:50:12 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 24 Sep 2021 17:50:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:645daffa61fcd5a11085215506814b0d0ca80fd670fb5a326e70db45a782120a`  
		Last Modified: Fri, 24 Sep 2021 17:52:31 GMT  
		Size: 4.2 MB (4219698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cce4d8baa6fcaed2284343b6cce6ff610bc7960c8fe2462d2429bafd5cbbc`  
		Last Modified: Fri, 24 Sep 2021 17:52:29 GMT  
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
$ docker pull nats@sha256:599a1dfd68ec271f0feb5380fc72a4ba9866c30c7f1d36dc4830ff7ec374de73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:5378bb9ab24c93ab0346dfaf7cd89a842513cb88c8f44680cb3e5045c085ddb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull nats@sha256:70a7bd523494ba4fededaca7552dd988ad31db63e5fcd1c24d0948cdfb4fb3b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692042587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9696f743cfec09dad17273758b713feda7277a5ee9b7e856ab938abf75015afb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:40:54 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:15:15 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:15:16 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:15:17 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:16:43 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:18:07 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:18:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:18:09 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:18:10 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:18:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c75402e6fab70f623ca8becfa5bb563e5630bbb4dac8adb11e385d75e171aed`  
		Last Modified: Wed, 15 Sep 2021 15:45:53 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72310736e43a0af90ac2e8cd43ae3c03f82f551700335ae1e3fb9227390a47f`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c169f31939e61fc36a0ae885f4b8a5e690baaabf3226c1eede24678385541db6`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e89355043258ee8779aab6bed36bf68ea3d11b091773a8231cecd5cc04e62`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef92d8b5dd739f491d14333a4e642017592f0a1ef40fca617fbc35f2a4e6d514`  
		Last Modified: Fri, 24 Sep 2021 18:22:31 GMT  
		Size: 366.1 KB (366064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aabfa02d0bb11bc462c049d8ad6334cad0d1ba8956d3c42730e8c254bd8c72e`  
		Last Modified: Fri, 24 Sep 2021 18:22:30 GMT  
		Size: 5.0 MB (4965459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e5825a2398d3273bc86df0e8bbf9ae99fe844e5b61ce929393fa3e785ebe79`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 2.0 KB (1972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b8e4397b768531a1faeff7623a8c5304f90c29905e5bef37f39459bb3802e`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f761ab7cc21ff4d80a14909bac8bc9c49f1a6611b221164104f9b84797ff396b`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198d5dde238d81b0642c12155d85314b1a644912fff89bc5726da1b7b2a67624`  
		Last Modified: Fri, 24 Sep 2021 18:22:28 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:75e4ff61015f3bf7c22351ff65fa904e8d4dc1323aa7f8881dfa10a7c2ffa49b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull nats@sha256:60236d944179b159cd056561c73729bb8eacaa25db732a8348c089e4553be641
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276661668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d133c7ce69a5c937d2c6fd5baba8fcea0547fe32f9caa257de095c5333b8fd7d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 15:43:15 GMT
ENV NATS_DOCKERIZED=1
# Fri, 24 Sep 2021 18:18:36 GMT
ENV NATS_SERVER=2.6.1
# Fri, 24 Sep 2021 18:18:37 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.6.1/nats-server-v2.6.1-windows-amd64.zip
# Fri, 24 Sep 2021 18:18:38 GMT
ENV NATS_SERVER_SHASUM=c98118acf708d119adb4d94127efb57825f24209e5e4b855931e3cc941237e35
# Fri, 24 Sep 2021 18:20:06 GMT
RUN Set-PSDebug -Trace 2
# Fri, 24 Sep 2021 18:21:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 24 Sep 2021 18:21:38 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 24 Sep 2021 18:21:39 GMT
EXPOSE 4222 6222 8222
# Fri, 24 Sep 2021 18:21:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 24 Sep 2021 18:21:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611fe9c559abed986280087eef7d362a6ecb9ad281b1427395fdfc2d99d3d9c4`  
		Last Modified: Wed, 15 Sep 2021 15:46:29 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326ce136baa17eaec1fac331c17c4cfccb1ab18ec89885c6e0a72acea536bd8`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3b1fed06b403050de165363f36dadfc9a9a527bbc7c077456a64f1d82c4d5b`  
		Last Modified: Fri, 24 Sep 2021 18:23:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cd472cc93732a042088cda0ff0d9bb6497ecf25c47d19333c1d5222e3d42e3`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b7607aa7457f0141c4f2f4ccacf4f068670acf5c00642aa11429b92c1d4182`  
		Last Modified: Fri, 24 Sep 2021 18:23:20 GMT  
		Size: 343.9 KB (343868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ef2571a70f7261d297cf7d19bbbddc950a9bc276fda13376fae1d091bc49e6`  
		Last Modified: Fri, 24 Sep 2021 18:23:24 GMT  
		Size: 5.0 MB (4976960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13f276de11afd9152b4309d095c5222ffc53d5f5000bd93f65ce3d0a8358b0`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd31e6f667b20a464061770ad947f5343d5c724176047276970528e29475ea1f`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b5018883280a197fb7725a0c7f6ce69f5a902ffa816ba93a509e98bef952c69`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d57908fe57f032c311e5df72827b4beb15403603b6d4047b329ad4b4cbd828b`  
		Last Modified: Fri, 24 Sep 2021 18:23:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
