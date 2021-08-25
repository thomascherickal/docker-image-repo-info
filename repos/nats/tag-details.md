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
-	[`nats:2.3`](#nats23)
-	[`nats:2.3-alpine`](#nats23-alpine)
-	[`nats:2.3-alpine3.14`](#nats23-alpine314)
-	[`nats:2.3-linux`](#nats23-linux)
-	[`nats:2.3-nanoserver`](#nats23-nanoserver)
-	[`nats:2.3-nanoserver-1809`](#nats23-nanoserver-1809)
-	[`nats:2.3-scratch`](#nats23-scratch)
-	[`nats:2.3-windowsservercore`](#nats23-windowsservercore)
-	[`nats:2.3-windowsservercore-1809`](#nats23-windowsservercore-1809)
-	[`nats:2.3-windowsservercore-ltsc2016`](#nats23-windowsservercore-ltsc2016)
-	[`nats:2.3.4`](#nats234)
-	[`nats:2.3.4-alpine`](#nats234-alpine)
-	[`nats:2.3.4-alpine3.14`](#nats234-alpine314)
-	[`nats:2.3.4-linux`](#nats234-linux)
-	[`nats:2.3.4-nanoserver`](#nats234-nanoserver)
-	[`nats:2.3.4-nanoserver-1809`](#nats234-nanoserver-1809)
-	[`nats:2.3.4-scratch`](#nats234-scratch)
-	[`nats:2.3.4-windowsservercore`](#nats234-windowsservercore)
-	[`nats:2.3.4-windowsservercore-1809`](#nats234-windowsservercore-1809)
-	[`nats:2.3.4-windowsservercore-ltsc2016`](#nats234-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:c3e75f817f347640bbfd05d134f47a0a04fe0df86265985e5e4ee9f5fbe72010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:a306b6fed9ddc40af4f29308e35543bac76b4a8912f864c07af9b4e8e0b77ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:20b14f999b9737575a787c9b37d4a3aeea37b0755c5cf57811c3cc3fc74c6dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f96d1ad611227df5c034ba26af420e318186acae8fcd998084ca42b76acd6607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3`

```console
$ docker pull nats@sha256:c3e75f817f347640bbfd05d134f47a0a04fe0df86265985e5e4ee9f5fbe72010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine3.14`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-linux`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-scratch`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore`

```console
$ docker pull nats@sha256:a306b6fed9ddc40af4f29308e35543bac76b4a8912f864c07af9b4e8e0b77ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.3-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:20b14f999b9737575a787c9b37d4a3aeea37b0755c5cf57811c3cc3fc74c6dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f96d1ad611227df5c034ba26af420e318186acae8fcd998084ca42b76acd6607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4`

```console
$ docker pull nats@sha256:c3e75f817f347640bbfd05d134f47a0a04fe0df86265985e5e4ee9f5fbe72010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3.4` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-alpine`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-alpine3.14`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-linux`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-nanoserver`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3.4-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-nanoserver-1809`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3.4-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-scratch`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-windowsservercore`

```console
$ docker pull nats@sha256:a306b6fed9ddc40af4f29308e35543bac76b4a8912f864c07af9b4e8e0b77ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.3.4-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:20b14f999b9737575a787c9b37d4a3aeea37b0755c5cf57811c3cc3fc74c6dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.3.4-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f96d1ad611227df5c034ba26af420e318186acae8fcd998084ca42b76acd6607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.3.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:d71a53fd0adacfb72039741fe307b54bed26b5bebc751a4e13d1087a87741463
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:7a1ec46ffffcc712a37d5e801e73e4cb68b22e15c842f36ab9211e1a039cb547
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7603979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:163732450f029c457fb0826ccdbb6d69696f0d8af625ed2bef5291b807563c38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:12:56 GMT
ENV NATS_SERVER=2.3.4
# Sat, 07 Aug 2021 00:12:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Sat, 07 Aug 2021 00:12:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 07 Aug 2021 00:12:59 GMT
EXPOSE 4222 6222 8222
# Sat, 07 Aug 2021 00:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:12:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6f975cea84a1db539a70743c469f460dfd3c0e9f53362581ea5166cc6f7bb`  
		Last Modified: Sat, 07 Aug 2021 00:13:34 GMT  
		Size: 4.8 MB (4790004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a3df61d2af8d57d3b1b9462ef7661cf873411724688e51359600bdddd950c`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7744cc9fd0f87944d530e0b43728226f13d0a9b61969249ab9b15dabd07d3`  
		Last Modified: Sat, 07 Aug 2021 00:13:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:29b04f6d57a29747dc657a7acc533ae6263d1f8fffcc8039cb9ab8a2f73735e6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7083280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abb28df26524d0f97b04d47d967afba7a509fba8a8e427d0cb8fd272b2ac90e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:01:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:01:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:01:53 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:01:53 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:01:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c84ab47f0270f4ad5be8602c279e3e42ad1b86ff081b41342dff0b989f1b342`  
		Last Modified: Fri, 06 Aug 2021 19:03:57 GMT  
		Size: 4.5 MB (4455962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b354f1843a75336b33fc518309fe07ddadb5cf05297d1c4f508a4e3b04a360`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150d7b64cd1b251621210455c6ef538c7d1b510891018c47f045feddf0024a99`  
		Last Modified: Fri, 06 Aug 2021 19:03:54 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:443f504d21f3881e958e0e58c996d3e5970ff90cf970c6e41adc2542ae14e2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6880695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671e9b1b37b7c31f58f233286cc6ee3009ae062bfd7634d1e8e15be89ea2492e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:26:24 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 20:26:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 20:26:29 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 20:26:30 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 20:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 20:26:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54864bfc951be8b12f75e7c53f918420224b41c45520c27dc54f47006e1ace61`  
		Last Modified: Fri, 06 Aug 2021 20:28:37 GMT  
		Size: 4.5 MB (4450364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e3d21fd5215bd4bad28c6e61f03fe72c301544f5e535f0f618132b4bf3d90`  
		Last Modified: Fri, 06 Aug 2021 20:28:33 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e584ceff2e79dca85ab2d5589768d2243a4b7e52b7e1743785667471c73d928`  
		Last Modified: Fri, 06 Aug 2021 20:28:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:3ba9b8c80c1026d2a500251c07a9af099943e0291f5c381e49e6d6e496f8de8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7115983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671a61b3bebfb1b125fc5ae67fc31351bc0aad1a0d1a103a21bb80895d7c09f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:49:47 GMT
ENV NATS_SERVER=2.3.4
# Fri, 06 Aug 2021 19:49:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 06 Aug 2021 19:49:50 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 06 Aug 2021 19:49:50 GMT
EXPOSE 4222 6222 8222
# Fri, 06 Aug 2021 19:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 19:49:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef6a8d5827e19307796e49f087f09097ca6784d2d680b67bf245e33eaa0417`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 4.4 MB (4404401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719578654cd35d6807367a487c4c618898557f046b46f894ccf6869b4d00cc`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742e4ce06ec6c0603f0ffe18a7788896b1ebe0f93184cba0be76177c3bb5c56b`  
		Last Modified: Fri, 06 Aug 2021 19:50:52 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:c3e75f817f347640bbfd05d134f47a0a04fe0df86265985e5e4ee9f5fbe72010
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:c191c7461bc7697ee6222d70680b57a59fdbaf1781a32102ae29004c0ef2e1b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:730384625ce5b4079ddcac6880f1490ee9597ae6bc21828aaa77fa16532f5c0b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107312800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc7723929ee86cd0b079266209ee6d5a7b6868ab2ccb6c25353fe3c894572a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:07:57 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Wed, 25 Aug 2021 16:07:58 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:08:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121849591f6022d5eb46ce6c232c4dd82c98ce40d0141bce3f4fd492ca1c7a59`  
		Last Modified: Wed, 25 Aug 2021 16:11:22 GMT  
		Size: 4.6 MB (4565853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ee09fe8225a9ce0552a9e934917caed425dfd666edee7135321ace67b098b4`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.6 KB (1614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba323a5abf6dad7d1a718aa3170520980aa1fbd31c381d54cc7471102fb2d915`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e3410faa2bff42c96e80f70ded6c98662c693d5110b30b9e8ea8e4d6323ba`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a3a7ef27ca50d4664393cf2b8e76b982f1169704081f714d56003e9fae41cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:17 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:633c08019ee754bb82987b4f6001dcbe7e415345d46d9eec34e5aa454e86b2fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:acd926de12a3d1a625d13dfab262fa240b0d99ecb35c68e372e093ab466d1b0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4506461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5738e29b3f24028140a48fe9652afc26b4118a35427b996d591872c6dd9162ed`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:edd123fab471ca4bff1ec55ddc839aaf0defe3667b337aaec7c3c8e70e903e8d in /nats-server 
# Thu, 05 Aug 2021 01:20:24 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:20:24 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:24 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:20:25 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3d02ec701f9917abde1e8953cba96577f89ebc29ced1af0d82734bde1a034361`  
		Last Modified: Thu, 05 Aug 2021 01:21:15 GMT  
		Size: 4.5 MB (4505985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beb29f4b4e73a454d8e38755b89ed0a71bb2f1aaaaa02105c3708af114c87cc`  
		Last Modified: Thu, 05 Aug 2021 01:21:14 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:684baaa35e7d8a0a37f5e62ff68dd3c3ddf62a523392a7b00f5b2440620681a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a518b2e63bf6fd16443c123d65a0a15f3860ba0601b9d8640ab7e3cef2a64f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 02:03:48 GMT
COPY file:1099ac4333f9709bdb701d77f49a9e3dfc443f1986fbf71cf0622f44b130cee0 in /nats-server 
# Thu, 05 Aug 2021 02:03:49 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 02:03:49 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 02:03:50 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 02:03:50 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:95139cea5d13d0e375a0e733a39d4f87cf133a9b2c8b9baf4cced90467ce4bbd`  
		Last Modified: Thu, 05 Aug 2021 02:06:14 GMT  
		Size: 4.2 MB (4174321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3970e4d2766394cc6ac0abee7ea43c436a324c9033b31b4116287a025feab571`  
		Last Modified: Thu, 05 Aug 2021 02:06:11 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:edbf04c6d86cc6973609fb90c099c175ba05216954d224ea93c03e862b6c0955
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4170312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d59f3755a610c7ef37ce7df6d7e2a6c1a1e7e0554fd7f0dfe5a7ba96370e6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:04:56 GMT
COPY file:f8d5a2ea993b24151d26b5967a44af43f6fa70afe6b7965767ebb48f41351935 in /nats-server 
# Thu, 05 Aug 2021 01:04:57 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:04:57 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:04:58 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:04:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0b65416c95f5f06a582f3d8ffe3f3cc9b4df10e5d724eb5167d7766bce64b77e`  
		Last Modified: Thu, 05 Aug 2021 01:07:22 GMT  
		Size: 4.2 MB (4169837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711811fab377fd6c12391460fafc4fe011d419669f5508b086b269489ae78d22`  
		Last Modified: Thu, 05 Aug 2021 01:07:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:258407bfd157b748b13d824daa441eeb795b46dae0dee509189e6f215219dfc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4121540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:928fc611a3e5935a6eea2e73e72cfc121d250a608f1def1e50e9a2bca5e9e0c4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 01:39:59 GMT
COPY file:e2687e43e0f0627dcdfb73c8b9b66c9a86cdda6399f627b485911acbece9a3c9 in /nats-server 
# Thu, 05 Aug 2021 01:40:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 05 Aug 2021 01:40:00 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:40:00 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 05 Aug 2021 01:40:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:333cb9b408ea509452b14ed5b1c9a8a6abed86e5a3177bc9ae7917d6c0c51318`  
		Last Modified: Thu, 05 Aug 2021 01:41:23 GMT  
		Size: 4.1 MB (4121065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b79f5ac7bd31304ad5fab87a7bb25e67ff6f7e8f0299806180b5bb556ea0dc9`  
		Last Modified: Thu, 05 Aug 2021 01:41:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:a306b6fed9ddc40af4f29308e35543bac76b4a8912f864c07af9b4e8e0b77ca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:20b14f999b9737575a787c9b37d4a3aeea37b0755c5cf57811c3cc3fc74c6dfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:6ccc9955cf40adb8ea2b253b9c6f23ec93119c186698e5ed532d40e6200d614e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691299672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a412cc016f80e4dadbe3a3dc5c2cb6a64665b0e6822a6da3cbb43db4b69bfe4b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:05:31 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:05:32 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:06:19 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:07:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:07:35 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:07:36 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:07:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:07:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce301f5f5d39ac4e8d9bcfbc328bd5b19ba33be4296e36dfaf38b97e237916cc`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd17b61217b895023497478b1741228ad7221f8c66e6112fad1b40bacc1ce5d`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94970df4678e54913d95980d02d9ff71d30d50a6723c96ec2a2c337d5ec94cc3`  
		Last Modified: Wed, 25 Aug 2021 16:11:00 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca036463e9405a39d3eecaf7c6d1460f43db9a3fb3a3a8ce3fa2a79129d9859`  
		Last Modified: Wed, 25 Aug 2021 16:11:01 GMT  
		Size: 372.2 KB (372161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3001228d4034679deb65e7813f9dad7e0bc52fa0888e3d8aabda79d824feca6`  
		Last Modified: Wed, 25 Aug 2021 16:10:59 GMT  
		Size: 4.9 MB (4916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4ad52d4d5186da25b2c5ee6ee1dece7dfa1006619a8c8dd61f03203bfb572`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bb136a83c4336ce77e23e25557549ed19968dd767ba7b9d2cc1e844eb6ba5f`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81fc52dc0eca24c32caca4700eda8838cb051b275a5522341356faa175af5f4`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5997d37eb36b34583172efc2d68231049fdbe4e1566a53766ab1dd9aeac733a6`  
		Last Modified: Wed, 25 Aug 2021 16:10:58 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:f96d1ad611227df5c034ba26af420e318186acae8fcd998084ca42b76acd6607
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:5f695f38c757cde6d2289cdba59daf5cedbed071bcd3b928c22b955fd45572a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276233135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:907eb440adcedcaa19bd8bda99341412fe2a823e1a7d3077d43d16c276523a2b`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Wed, 25 Aug 2021 16:08:07 GMT
ENV NATS_SERVER=2.3.4
# Wed, 25 Aug 2021 16:08:08 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Wed, 25 Aug 2021 16:08:09 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Wed, 25 Aug 2021 16:08:54 GMT
RUN Set-PSDebug -Trace 2
# Wed, 25 Aug 2021 16:10:15 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 25 Aug 2021 16:10:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 25 Aug 2021 16:10:17 GMT
EXPOSE 4222 6222 8222
# Wed, 25 Aug 2021 16:10:18 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 25 Aug 2021 16:10:19 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9a660f8d67a5c8b9457024d09e515ec58c8139030455fad6d652311b6efe4`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03452b1283e873ff333ca54ed6173a3903c0ee3a0d275877acbe830baba2300e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d20a02f5d333ae12d83abd2efbb61180409c8fc087bbfae23a15333093bfd`  
		Last Modified: Wed, 25 Aug 2021 16:11:40 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6996d861cc65b368ae3430040a02f90e24442c11c36ba92e60ca871ea2ea2e4e`  
		Last Modified: Wed, 25 Aug 2021 16:11:39 GMT  
		Size: 337.3 KB (337279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1a3283ad2e2971b500f94eddc08246fe108cd32ace09dc8d975000b95a7ef6`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 4.9 MB (4917237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee3ec74d5606f197fc248615bc3f601b7ead0dfeec128858be0db44a480d5c2`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.9 KB (1852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eee0b51f0797517ba761ef6dbba5511ca115f27a7fed19265c2547da9697b`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec6d361ef3b2338bd83a5d1f88667ceef00c4882ba2b9f425305114c0093802`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac609389baf550f0bab83b6b5bc067bf62486e9bc22d12b12c9d0866fbacb48`  
		Last Modified: Wed, 25 Aug 2021 16:11:37 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
