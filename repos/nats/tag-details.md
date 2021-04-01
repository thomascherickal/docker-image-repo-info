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
-	[`nats:2.2.0`](#nats220)
-	[`nats:2.2.0-alpine`](#nats220-alpine)
-	[`nats:2.2.0-alpine3.13`](#nats220-alpine313)
-	[`nats:2.2.0-linux`](#nats220-linux)
-	[`nats:2.2.0-nanoserver`](#nats220-nanoserver)
-	[`nats:2.2.0-nanoserver-1809`](#nats220-nanoserver-1809)
-	[`nats:2.2.0-scratch`](#nats220-scratch)
-	[`nats:2.2.0-windowsservercore`](#nats220-windowsservercore)
-	[`nats:2.2.0-windowsservercore-1809`](#nats220-windowsservercore-1809)
-	[`nats:2.2.0-windowsservercore-ltsc2016`](#nats220-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:4cc6ae97db8f844bcb32288362ff30125146324890be158dc006e0d6bc7d4a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:20cf55d646dc015d67cf875917303b92617df0171995ba47d6b618e4e529ac0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:7b2fbe5ca6f19a967f05ffe532bf7773615ac93729f5692f79c3b0b217f93ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3834fa2834ff7755787b18e5da79d4cc1ac5993bd67a652048db5fe9f8f6e94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2`

```console
$ docker pull nats@sha256:4cc6ae97db8f844bcb32288362ff30125146324890be158dc006e0d6bc7d4a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-linux`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-nanoserver-1809`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-scratch`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore`

```console
$ docker pull nats@sha256:20cf55d646dc015d67cf875917303b92617df0171995ba47d6b618e4e529ac0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:7b2fbe5ca6f19a967f05ffe532bf7773615ac93729f5692f79c3b0b217f93ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3834fa2834ff7755787b18e5da79d4cc1ac5993bd67a652048db5fe9f8f6e94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0`

```console
$ docker pull nats@sha256:4cc6ae97db8f844bcb32288362ff30125146324890be158dc006e0d6bc7d4a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.0` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-alpine`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-alpine` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-alpine3.13`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-linux`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-linux` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-nanoserver`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.0-nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-nanoserver-1809`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.0-nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-scratch`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-windowsservercore`

```console
$ docker pull nats@sha256:20cf55d646dc015d67cf875917303b92617df0171995ba47d6b618e4e529ac0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2.0-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:7b2fbe5ca6f19a967f05ffe532bf7773615ac93729f5692f79c3b0b217f93ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:2.2.0-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3834fa2834ff7755787b18e5da79d4cc1ac5993bd67a652048db5fe9f8f6e94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:2.2.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:ece4acb6a22288af4da0016e4af11c093f935d2d68ed74fd5b4b88869dd292c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:faf06335ff05259553a7cd85c508540576e73735f878f991bdb316639c5beba8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baae0ba3d35d13f1ab017cea5d7a4c34e55d533b5f83ee0887f4e46b9df6169d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:29:19 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 14:29:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 14:29:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 14:29:23 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 14:29:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 14:29:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada4cf180db02bbf5a645d367b3c999bd2d866adfb6969b459025ab3a5f5865d`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 4.5 MB (4465448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b817b47391bfd1cb047c312e74ba8c28ef3055a3f2610b6e1cac5fdb07d259`  
		Last Modified: Thu, 01 Apr 2021 14:29:59 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66852cd6a6ebc8a62018430b7b8048a2a6a6c95a33d89e73450ee3821b2eefb2`  
		Last Modified: Thu, 01 Apr 2021 14:29:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:176e8d0085b947261153305c1788facc818e70e077179cad7508f5f43bedf77e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9af42585046c70139fb1bb86197b2a6bb68b7a63929d91b30d560ef385d96fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 19:52:22 GMT
ENV NATS_SERVER=2.2.0
# Wed, 31 Mar 2021 19:52:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 31 Mar 2021 19:52:29 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 31 Mar 2021 19:52:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 31 Mar 2021 19:52:30 GMT
EXPOSE 4222 6222 8222
# Wed, 31 Mar 2021 19:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 19:52:33 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82bb4a6b0c990fafb5aee813c8eb708a86505f095c25955d88163310817dc513`  
		Last Modified: Wed, 31 Mar 2021 19:53:15 GMT  
		Size: 4.1 MB (4140807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcd67a5460afa2ecd7ff1f09dbffa0a3ee971b3c9211781b47f018dfb18604b`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e265ad0375bb3e77396d2def17dfd4b28486975504690db16fe5e3379d72c149`  
		Last Modified: Wed, 31 Mar 2021 19:53:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:0d0d69075781a3105d70b4607557c74d2c13430f137da5d4ad9b893ff47bbcc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb0c3f1895fa95164aab25913ef37b6488bb4ef685b45fc7ea757d2028570cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 09:52:30 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 09:52:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 09:52:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 09:52:37 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 09:52:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:52:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d72610fdeddca533a7fa8937e70712fae7aca0dcb07d6fbba1e43b20190fe8`  
		Last Modified: Thu, 01 Apr 2021 09:53:21 GMT  
		Size: 4.1 MB (4134981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12af5140a82cb853be34ad036db9ac6e67f64654816fb140706e62e9c49dec4`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56601effdbab268d5f96f091e3ab569209092f832637c2f53712cdd0c4cb06e9`  
		Last Modified: Thu, 01 Apr 2021 09:53:20 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:5e40ddf9a4d4f163f9f413a0a749d385b437a598d53ab8c462d21e6df734c97d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6822164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbc27f239e9627f70c924bbb76c70b230bfabe5e49e3a7d9df731e4f38f39a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:43:27 GMT
ENV NATS_SERVER=2.2.0
# Thu, 01 Apr 2021 13:43:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 01 Apr 2021 13:43:33 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 01 Apr 2021 13:43:34 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 01 Apr 2021 13:43:34 GMT
EXPOSE 4222 6222 8222
# Thu, 01 Apr 2021 13:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:43:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7065a6411f04b75bef4097e4ddf4951d84ad0bfe9c9d9552a92bf75a42c77bd9`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 4.1 MB (4109274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db97b33cea8fa80f73c926008de131699a2fe7671dd699420d9c86a98a4c47a`  
		Last Modified: Thu, 01 Apr 2021 13:48:40 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c025cd8f41b22d6bda55a9235f10bf1751237ebff13e7ad89ed1325fbc9d86e2`  
		Last Modified: Thu, 01 Apr 2021 13:48:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:4cc6ae97db8f844bcb32288362ff30125146324890be158dc006e0d6bc7d4a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:0952bb16a502372a4b3637620ad4b23f1cd1658ec3a202fc8e4997d884e1da21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:3621f57fd3c277ec4cbe88e91a364bb90b3a614178b075b262025c69902f6749
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105632823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a15211278567816e8c2d0069b2ff094c0b9dcb8cf04e2d51d41006e2004719`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 16:56:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:12 GMT
RUN cmd /S /C #(nop) COPY file:ae552f9fffc5cd2f6ed45296e57705c2f61343b2c0e5351c85ccd047adfa7b73 in C:\nats-server.exe 
# Mon, 15 Mar 2021 20:17:13 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:17:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:16 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f49969195f32b7e40a81e3d189259fec7ebf52ee0ec5dafd5f3f288715354fed`  
		Last Modified: Wed, 10 Mar 2021 17:01:57 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8ae67f49930ee74c376428149104959d1ff9583b9fdbb41fdb5aed581931f2`  
		Last Modified: Mon, 15 Mar 2021 20:22:15 GMT  
		Size: 4.2 MB (4236588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f29b29488ecf17138eea47d55def6573211a3f9a3e68a1fa63e5cd412339d2`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.8 KB (1773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3d7ef6e3c578d1823bbe7699b42e32f024d0b5de366ce42cf2cfd46ad2f76`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa0a814bb44d3fb408de44b16509731ff63e96cea480295bb63dfc15fe5789`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d3b5144a635921fbead0a95e2d3a141eddba274abd7c281b40fadc3d13e121`  
		Last Modified: Mon, 15 Mar 2021 20:22:14 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:1bcf420793f93ebc2a34ce16e797f78fa698659f4257a29ef3240567cf149ae8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:ebea070618f2459bc2f6a200dadc2f1a4c0763212c361372b62e98660433e12b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4185085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bd9298a0432fe41651ac7852910e0de92e1bde3bd7497195ffc861b4785d3f0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:b5d1e003164e33741898b7ec26a4040874906b36efbc359506c187ae6df7c294 in /nats-server 
# Mon, 15 Mar 2021 20:38:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 20:38:15 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:15 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 20:38:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:061215568e0623f6f43c6616f33a9bea7665a183db6a276a6038af3f305833d6`  
		Last Modified: Mon, 15 Mar 2021 20:39:10 GMT  
		Size: 4.2 MB (4184610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05331b79a067343f06d2c17089ee22d3cd8193f712ae7647b0977867e36bc36a`  
		Last Modified: Mon, 15 Mar 2021 20:39:09 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:81a7d3301eb008ada26d22889711a883bbad763673b54f7593f2445d22298acd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3859233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8dc88c3bd1fffabc0615fa001fa033818d9eee65d62c50afed1958c58045ab4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:17:04 GMT
COPY file:d436e7cf1178e7919a5eeaba22715cc73a25f54e3b98dc4c2511f0969af50c7d in /nats-server 
# Mon, 15 Mar 2021 21:17:05 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:17:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:17:07 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:17:08 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:029a8ef0b1c1c9cd107dd578ac757718ad474948fd5e7b25aacc28f3507dca3e`  
		Last Modified: Mon, 15 Mar 2021 21:17:49 GMT  
		Size: 3.9 MB (3858758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3658434d7560f8e07a195f69d5fca2be87c52936bbebb0443bb8d30b36aa0072`  
		Last Modified: Mon, 15 Mar 2021 21:17:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:b2e5433b90b1cdd96decdc44183063bffcc7b73e088c1033edccb1afd8a5c17f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3855937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b8659db05958c00c35ed9fbd5356e048d3585f6ab0de6b4ad63250f013741f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 21:24:57 GMT
COPY file:68bb849e5773af4031f3eed004a40bf4f742c3945319085d56bee16a0a9207d2 in /nats-server 
# Mon, 15 Mar 2021 21:24:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 21:24:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:25:00 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 21:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e6b2bfbd8fee738af6e2eb535451184e1cfa44d6189259fc78a03247687a7a3`  
		Last Modified: Mon, 15 Mar 2021 21:25:48 GMT  
		Size: 3.9 MB (3855460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5a766cb9431ee6ca3fa9462f0b1cd15de1270719b74fe5f17e3bbbf75acbc0`  
		Last Modified: Mon, 15 Mar 2021 21:25:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:68284dadffb40430476fffec3f3f3175e215e0efbd8ebb3b84d61745afbc8208
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3826067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9c42fd7b12781200e6e26a21ac0f074a31c2bb3ab913378dbbd126c5e1dc232`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 15 Mar 2021 22:15:07 GMT
COPY file:cc5a975f9a3d3dec9e7c117963cb0f29cccd7a6d9891efe13202d82f16983d97 in /nats-server 
# Mon, 15 Mar 2021 22:15:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Mon, 15 Mar 2021 22:15:09 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:15:10 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 15 Mar 2021 22:15:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6dfc8ec71d6cbeecdf9b73546e133c54fe31a144e705660e1732d4c3fd7cec38`  
		Last Modified: Mon, 15 Mar 2021 22:16:28 GMT  
		Size: 3.8 MB (3825589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8298fc0383beb85f28b7722738f7772924405727f566aba126c37b60b6fb55d4`  
		Last Modified: Mon, 15 Mar 2021 22:16:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:20cf55d646dc015d67cf875917303b92617df0171995ba47d6b618e4e529ac0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:7b2fbe5ca6f19a967f05ffe532bf7773615ac93729f5692f79c3b0b217f93ab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull nats@sha256:6d99e95fff4ff767ab455c72aa0361e2607d0e869cd0ebc03108d6ebe754a0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2480270595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39eb19c744ee00d943aca95c0fa139702f823a1d2a6c29284a88efbc92dff715`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:54:55 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:15:09 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:15:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:15:11 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:15:44 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:16:57 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:16:58 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:16:59 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:17:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:17:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfde5dabd6353190a5343286e79ed9ad72f47f48ca9197e594b9771b5039e7d`  
		Last Modified: Wed, 10 Mar 2021 17:01:37 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c501e38cf1bef759506cac477656d1525304d314d1a87272b2e5a0d9340ec`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3a3e3973ec4905795d6f69337230ae1a3ffa39b5e67e3218240c9d81767f30`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9182aecd18e9366e616d956594c87a9ec12af89cdb5174b5e44491595b993f44`  
		Last Modified: Mon, 15 Mar 2021 20:21:50 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f873dc755700e152b9e36bdf8e52acd3c0b3f89834258861ec7b63cad2f83e`  
		Last Modified: Mon, 15 Mar 2021 20:21:56 GMT  
		Size: 5.1 MB (5065010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b58dffd304059fbf01e8f232cae78694b01f59492227e635b13f4146e5398de`  
		Last Modified: Mon, 15 Mar 2021 20:21:51 GMT  
		Size: 13.7 MB (13658048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1636b7b5c5e6f053527b20437d39447a1784781d3096d989e47565502c2a24`  
		Last Modified: Mon, 15 Mar 2021 20:21:48 GMT  
		Size: 2.0 KB (1955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3c66b0dc873dd0d4229a873a8159b0f5cede6052128b2801276a929425d83`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a4f11cb5d2d425ca56aa82fb6143e429ff6b4a1fdce2c446c0cd47c21f8c`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f5314021a971f3e889e272e828fecd71afa4737daaac51ff38997e799940d2`  
		Last Modified: Mon, 15 Mar 2021 20:21:47 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:3834fa2834ff7755787b18e5da79d4cc1ac5993bd67a652048db5fe9f8f6e94c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull nats@sha256:dff89ffda8b40b781df892c7c718b15a74e1b36f494dbf2ad90e7452ecc62ff2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5817000223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c590e9cb4ced34c77d451c8a89d263bb88a3e585734a8fb8b5b6e757282d49a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 16:57:09 GMT
ENV NATS_DOCKERIZED=1
# Mon, 15 Mar 2021 20:17:26 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:17:27 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.2.0/nats-server-v2.2.0-windows-amd64.zip
# Mon, 15 Mar 2021 20:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=60d10965b1902baab48d9ff621a4a5504c8fa29d0a9543d5e683d0b8059b62b9
# Mon, 15 Mar 2021 20:18:51 GMT
RUN Set-PSDebug -Trace 2
# Mon, 15 Mar 2021 20:20:55 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 15 Mar 2021 20:20:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Mon, 15 Mar 2021 20:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:20:59 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 15 Mar 2021 20:21:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390a91a59ec3760f5740301d69b960d0f0b7fb212a8bc2201b27b93b24d4054`  
		Last Modified: Wed, 10 Mar 2021 17:02:23 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dd615c71b4eb4a71c45a379e363133bbb592ced1d774829054c1bcbf02c424`  
		Last Modified: Mon, 15 Mar 2021 20:22:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45de2ae9457cb71c5bb1e8bdb53c2b939780bb3464988803dca8de78d26e6466`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d31805eb5a4d29293c5e38dfdeded0848951ded5074473f16379814ad721dfa`  
		Last Modified: Mon, 15 Mar 2021 20:22:34 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1821fcfe740d7a4d72ebce808af7aab6d489ed0ebb05a3267af44b6ecdd077cf`  
		Last Modified: Mon, 15 Mar 2021 20:22:41 GMT  
		Size: 5.7 MB (5657003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5450f7da02165757aac5e164ed5942b0d00029e6640e4381b387e0e385928f0b`  
		Last Modified: Mon, 15 Mar 2021 20:22:36 GMT  
		Size: 14.4 MB (14419153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcc2db76c93f9eb235e225a970ef65b1af8da4bff671559ed6c69083ebe489`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52e6deb4edd19df80782ba9567175f929679b82d28178ecb8abe5d9148a429d`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b683bc157b68668fb555d38ed7784efab9518ab6d38c3021ffdebac80a849a`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2f56628b687521cdb1e451f56f34abe807cb72da1a00c1c16c00e82adf9702`  
		Last Modified: Mon, 15 Mar 2021 20:22:32 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
