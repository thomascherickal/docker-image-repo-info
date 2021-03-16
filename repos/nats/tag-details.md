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
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.13`

```console
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
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
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2-alpine3.13`

```console
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
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
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-alpine` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.2.0-alpine3.13`

```console
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.2.0-alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.2.0-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
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
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.13`

```console
$ docker pull nats@sha256:04056aae6c6ae545f8a1e126c8a861e9b9533ed7f14949e4fe9e9769821dd073
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.13` - linux; amd64

```console
$ docker pull nats@sha256:0588bdd49eff9fbe5a97b3e59d8be059b2a3e28fc10028e5acc783c04168af62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7278086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54139de8fa56bbc2ccf30efcab4bf2ac3d8fbd197fafdb1227536ec200fbd28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 20:38:02 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 20:38:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 20:38:06 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 20:38:06 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 20:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 20:38:06 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de6c88bd8bb61feb100dc546a639f394479b63ab77b85b204b919c037e3561c`  
		Last Modified: Mon, 15 Mar 2021 20:38:45 GMT  
		Size: 4.5 MB (4465460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c16ca1333387827028b48699ebf7705fec9cba68418e481f6844a7a5ce84a`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363cd9ab055c3a7affd93e67333d1bbba811b592ec3c1dc8a0b449d14392ffcd`  
		Last Modified: Mon, 15 Mar 2021 20:38:44 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v6

```console
$ docker pull nats@sha256:3b09aaa49e9ec674f064d69adde7ff3746fac00a4dfcd49c74bbde754a6486a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf1914719a1adcdac67b8cf15e7cf6f3c3f520405439a53770af13c049b7966`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:15:53 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:15:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:15:59 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:16:00 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:16:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:16:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303c38c75c792b3baa6a38dd076a2776c8f9fded9e8b2d7922b82e65463b66e`  
		Last Modified: Mon, 15 Mar 2021 21:17:35 GMT  
		Size: 4.1 MB (4140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822378818180c446dcc1dbaf6cf750ce747aa292fd991f1844e83b23249db84f`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dbd40dab87b34d2855c1f53815d15407c9e80ae40ab94d258c4c88d1271c00`  
		Last Modified: Mon, 15 Mar 2021 21:17:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm variant v7

```console
$ docker pull nats@sha256:b864b2dd1d22aa7b79f42ac9e76d8a2cf236482a1a80366dd63d147cfd836c11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6559845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:362b7a041a42201c7f0f1e90623dd37ab077b5c5acb6596403e36ab6abadedf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:57:36 GMT
ADD file:efdd39e5243eaf378f12ad5a85d2222b44930850a90263e5f17e8a6b5e9bc9b8 in / 
# Wed, 17 Feb 2021 20:57:37 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 21:20:49 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 21:20:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 21:20:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 21:20:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 21:20:57 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 21:20:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 21:21:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f55b840e27d3dbe27e44497103a4397f043749f933eb0433d29e2f104b3435ef`  
		Last Modified: Wed, 17 Feb 2021 20:58:14 GMT  
		Size: 2.4 MB (2423892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27d2f1024ee6f137f679cc66d38363972f76824d87b5f16e4a751e6845f297b`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 4.1 MB (4134980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661d8a6cd44e4d001074e3f9da0ff480efb9de0846813635dba6b267eff76177`  
		Last Modified: Mon, 15 Mar 2021 21:25:30 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3426dd5b3f09fb5c0e8e720c12de50ab3890f37d36deb9198f5e5680232ac4e8`  
		Last Modified: Mon, 15 Mar 2021 21:25:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.13` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:ba5427cdb73e45d940e785bc123b0ecc0fe7aacb57e7222a188b75f29c54adf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6821717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034dc01fad63fe260a0f644d8dda705c2c7658723244366989f4b8e17d23c0b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Mon, 15 Mar 2021 22:09:42 GMT
ENV NATS_SERVER=2.2.0
# Mon, 15 Mar 2021 22:09:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4dfcf480a32d9ba7098477387d96a657a036ef9ad495a008a83e06b22df63999' ;; 		armhf) natsArch='arm6'; sha256='b82fdb2c8f6e7c731254730043c145423b5c48a3b40e33ad6e32bce029a9f086' ;; 		armv7) natsArch='arm7'; sha256='cffc326c7faeb5ea0769d0f04787d9885d5b2baabd32000d3b18b1130742772e' ;; 		x86_64) natsArch='amd64'; sha256='764ee4a9761185f92904c21c3de204c8b898e9a6bad6afac8b1fe512ce887417' ;; 		x86) natsArch='386'; sha256='a8067d9f26007bed3df2a72eebd4a813035a473058db1451d615ef5e96b30577' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.zip "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.zip"; 	echo "${sha256} *nats-server.zip" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp unzip; 		unzip nats-server.zip "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server"; 	rm nats-server.zip; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rmdir "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Mon, 15 Mar 2021 22:09:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Mon, 15 Mar 2021 22:09:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 15 Mar 2021 22:09:50 GMT
EXPOSE 4222 6222 8222
# Mon, 15 Mar 2021 22:09:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Mar 2021 22:09:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47184a8d6e652e9c3893688cadcfaac678dd9bba677246459c0451b14a53bd`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 4.1 MB (4109175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65589fd772e58c1aa03b1b49be83fa3909c9db60a4b8b10670b8ae85292e884`  
		Last Modified: Mon, 15 Mar 2021 22:16:07 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd62fd1ff9c979fd53e99f28463065043c4cf0dc1091e2d7490bcca2e646eb3`  
		Last Modified: Mon, 15 Mar 2021 22:16:06 GMT  
		Size: 412.0 B  
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
