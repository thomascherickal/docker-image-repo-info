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
$ docker pull nats@sha256:cbad238c7c448fbbfca640e7c1d16892080706bf185287d4c873a6ab8ee4b44c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats:2` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
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
$ docker pull nats@sha256:8a2f2b63e9b923e448d7ae445b02d1fad6a450bdb759184b2876bb3252764ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:7bc91025d330e69dbd5130de2ef309126249f780ecb8d3951b7c6dc27118b8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7d611980e8b0160efe98f0d693f97b1733f156f87a1fbba62f20d8264d2296a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3`

```console
$ docker pull nats@sha256:cbad238c7c448fbbfca640e7c1d16892080706bf185287d4c873a6ab8ee4b44c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats:2.3` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine`

```console
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
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
$ docker pull nats@sha256:8a2f2b63e9b923e448d7ae445b02d1fad6a450bdb759184b2876bb3252764ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:7bc91025d330e69dbd5130de2ef309126249f780ecb8d3951b7c6dc27118b8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7d611980e8b0160efe98f0d693f97b1733f156f87a1fbba62f20d8264d2296a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4`

```console
$ docker pull nats@sha256:cbad238c7c448fbbfca640e7c1d16892080706bf185287d4c873a6ab8ee4b44c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats:2.3.4` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-alpine`

```console
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.4-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.4-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-nanoserver-1809`

```console
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.4-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
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
$ docker pull nats@sha256:8a2f2b63e9b923e448d7ae445b02d1fad6a450bdb759184b2876bb3252764ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3.4-windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.4-windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:7bc91025d330e69dbd5130de2ef309126249f780ecb8d3951b7c6dc27118b8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:2.3.4-windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7d611980e8b0160efe98f0d693f97b1733f156f87a1fbba62f20d8264d2296a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:2.3.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:54ba51d16eb88691dd858d083012cd325c90025a679e18fe75496569f21286ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:aa8d6df107099e3d50f98a8bfe9f7e4c52023f0c0f5f0bc5ee89d775792e9ed0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7602455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01640f492e23993e18e6c586c03a9c23b9129a296e8d8e02b4d5422740863e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Thu, 05 Aug 2021 01:20:12 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:20:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='c8ba676a6c4ec9d3088e0b64ffdae36e2f2a9e1b89f030799f3efbb2923524a0' ;; 		armhf) natsArch='arm6'; sha256='d1f14441d1fbd53a7bff9623e8e572707d3e7024b42b6e925ad371d4dec0bc47' ;; 		armv7) natsArch='arm7'; sha256='2488706de91e94eba477ddbc3b293ec0b4d823509656cc101eec6a07e0319bb5' ;; 		x86_64) natsArch='amd64'; sha256='8c11abdeca4882888a8b6fbc45effe9fb4d1070eda3939b7299892c8c69a3e87' ;; 		x86) natsArch='386'; sha256='010bca73095d8a05495ef74a112dfd3919925b0ced10bc4c5f876f3858ca41f7' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 05 Aug 2021 01:20:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 05 Aug 2021 01:20:15 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Aug 2021 01:20:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4bbee8f25494718730aa5ebff74dab60f38f303e988e4a7eab989ba0669a7e`  
		Last Modified: Thu, 05 Aug 2021 01:20:51 GMT  
		Size: 4.8 MB (4790007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae6ecbeb5464957754cc177cbd4fc5a4e8eff3ebda4089210368958dffbf88b`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c127bfb05be78a521551387911d85895dc91150ef7e5d40add61fe00d2dc5`  
		Last Modified: Thu, 05 Aug 2021 01:20:50 GMT  
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
$ docker pull nats@sha256:cbad238c7c448fbbfca640e7c1d16892080706bf185287d4c873a6ab8ee4b44c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64

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

### `nats:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
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
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:202fe1d65b01bc9c3cfc84851b13e703fab550b4fac1694e97b736c22c3f1417
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:ee74123de476443382107d6aac1f65501bb5af6241e5ca7c5917514bba0665b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86122d08689fb286513b0a4b6819ca71ef9415580a8f108b3e2c2645577b0d94`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:07 GMT
RUN cmd /S /C #(nop) COPY file:8538955caf7c9caa9eb4d7b28f10bc92a634b0dd46f131100d399a0d3ecf12e3 in C:\nats-server.exe 
# Thu, 05 Aug 2021 01:17:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:17:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:17:14 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9cf5e9423387ba0d3b7fa92275ffe5a4dcb519ba10e56c694d139e2e821f4`  
		Last Modified: Thu, 05 Aug 2021 01:21:06 GMT  
		Size: 4.6 MB (4565934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2932ac99aff67d8bd2497ba5a22bc8a1161b52fbee2e76b4825b40c5fdc70`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4f754dc3a014fade0d9fd62fbda58619ea01ab9627ef25bfec7f6626d8500c`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b6d1d7c23526680c2c77d926460333000320c8b6c786d281d27d86f85a137`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63df2e6e08a1bee7bce987dd3e56ff9d4ea9d582b071d6107ed5bd610ccfc42a`  
		Last Modified: Thu, 05 Aug 2021 01:21:05 GMT  
		Size: 1.2 KB (1163 bytes)  
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
$ docker pull nats@sha256:8a2f2b63e9b923e448d7ae445b02d1fad6a450bdb759184b2876bb3252764ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:7bc91025d330e69dbd5130de2ef309126249f780ecb8d3951b7c6dc27118b8b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats@sha256:9e2d731cdb925c898d4579320d72701d2ac4fe6364d4eb2bca58ed40532cc2a5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2690732563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ce9dae20e0206a3c75271c45ca7b3b6ae85b1fddbbac124fe498e4597d1fa65`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:31:26 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:14:25 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:14:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:14:29 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:15:28 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:16:45 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:16:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:16:50 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:16:52 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:16:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92bdc410321db22d4cf09322869bd9fb2495788c3725624c86d76a6ab3d95d3`  
		Last Modified: Wed, 14 Jul 2021 02:40:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5979713f8e1f662fa1588049500ad9a02d8f21edadb4270f498e66188c7f098b`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbce67e3f27ea6f2ced1a18b80f76be1d1d9f4a3360eacf9b682f76e22ce70bd`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cc6410be930a503a8d84a6c5179fc77d4f264b575a6b8ed9dba8652130448`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf5b9d1c9be32f37073b8570c4f5425741bf087b26830f109cf1da7548b2d4`  
		Last Modified: Thu, 05 Aug 2021 01:20:46 GMT  
		Size: 364.0 KB (363963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630752cfb4d0af660aec8e61449bdee0768f832622c426e164c52310feb34ea`  
		Last Modified: Thu, 05 Aug 2021 01:20:49 GMT  
		Size: 4.9 MB (4908534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974b95416575ac8447156b16b48dbc2c1075da313fb92b34649907cfa9e64f6d`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732a55fe045a7122347b15fe0ffeb6f778d44005ba9fd8895a5742b53a3b45e3`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750ae0f00a0b9b06b5540e999091d41c325666fe51da95ef04aac1a4677dccf1`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420ec40c0c7e96c3c2c8c8e4eb016f945ebe02a4471a1acad0d1b870447ba3e`  
		Last Modified: Thu, 05 Aug 2021 01:20:43 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7d611980e8b0160efe98f0d693f97b1733f156f87a1fbba62f20d8264d2296a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4530; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4530; amd64

```console
$ docker pull nats@sha256:d6a80df594b9c79713e2e081ee4745d866c2e22d200cf6c6313bcfd3c11dab24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6274950599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6d32b272b39dcd6b458d9516034bb382ae8d518db805e3fbcf74057d97981a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 02:35:48 GMT
ENV NATS_DOCKERIZED=1
# Thu, 05 Aug 2021 01:17:24 GMT
ENV NATS_SERVER=2.3.4
# Thu, 05 Aug 2021 01:17:26 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.4/nats-server-v2.3.4-windows-amd64.zip
# Thu, 05 Aug 2021 01:17:28 GMT
ENV NATS_SERVER_SHASUM=729dc0609e0461aa5fb893c85c04c6b6afa40945183d8d8324d03186d1678a99
# Thu, 05 Aug 2021 01:18:30 GMT
RUN Set-PSDebug -Trace 2
# Thu, 05 Aug 2021 01:20:04 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 05 Aug 2021 01:20:07 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 05 Aug 2021 01:20:09 GMT
EXPOSE 4222 6222 8222
# Thu, 05 Aug 2021 01:20:11 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 05 Aug 2021 01:20:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf08cae8b8db8f3f89e1a9192d393f2da55b44efce4e778fdb58debe2d608275`  
		Last Modified: Wed, 14 Jul 2021 02:40:57 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c44d1c9a8f9d7ad841c012f6de896b6b36c94f648f369709ec714de6a0561`  
		Last Modified: Thu, 05 Aug 2021 01:21:25 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a36861d11e97c8f3cd60182e69d6547fd3c7dd681fd5b892bf674d263cfa55`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2af8594f437c6c2c3ae701f3a8ef3f49d2860254568fe9cdcb902236a8b2ea`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847d098f9f9ff94b78c44a267a8eee1f258171e94527ef03da4e0a2e4630720c`  
		Last Modified: Thu, 05 Aug 2021 01:21:24 GMT  
		Size: 364.9 KB (364876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce96aca778ab04bb9b2b258bb6c0b4af50f1293387a21bb7ecab954e1df51f7`  
		Last Modified: Thu, 05 Aug 2021 01:21:23 GMT  
		Size: 4.9 MB (4940388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86c1babce557e9804d282d3f84516018239e1953d2f331882c347ab4405c0af`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac7eea6fd5241c5e955f00a169cfbec20397f9a877ccef20e110666b809032`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f36c1ea25dfc115b0ec159e748c702ce956653eda92844ecf60770259892cc5`  
		Last Modified: Thu, 05 Aug 2021 01:21:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36bfc5e3a0934ddca0f2028862fe5255420db252cc34f75fcd7707565180e3a`  
		Last Modified: Thu, 05 Aug 2021 01:21:22 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
