<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.16`](#nats2-alpine316)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.16`](#nats29-alpine316)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.6`](#nats296)
-	[`nats:2.9.6-alpine`](#nats296-alpine)
-	[`nats:2.9.6-alpine3.16`](#nats296-alpine316)
-	[`nats:2.9.6-linux`](#nats296-linux)
-	[`nats:2.9.6-nanoserver`](#nats296-nanoserver)
-	[`nats:2.9.6-nanoserver-1809`](#nats296-nanoserver-1809)
-	[`nats:2.9.6-scratch`](#nats296-scratch)
-	[`nats:2.9.6-windowsservercore`](#nats296-windowsservercore)
-	[`nats:2.9.6-windowsservercore-1809`](#nats296-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.16`](#natsalpine316)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:194a8dab745155aa91ab7a025ec1b6462cd95ef1aef0c736b20fbb717c1defa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:194a8dab745155aa91ab7a025ec1b6462cd95ef1aef0c736b20fbb717c1defa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6`

```console
$ docker pull nats@sha256:194a8dab745155aa91ab7a025ec1b6462cd95ef1aef0c736b20fbb717c1defa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9.6` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-alpine`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.6-alpine` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-alpine3.16`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.6-alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-linux`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.6-linux` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-nanoserver`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9.6-nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-nanoserver-1809`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9.6-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-scratch`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.6-scratch` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-windowsservercore`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9.6-windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:2.9.6-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:44effbc5c239cb864bb79bca5eabfb1d80862950b83ccd44e949b68e98398b5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.16` - linux; amd64

```console
$ docker pull nats@sha256:80f0115de5ee5eb05c78d116eea70cc91aee8fc32a5c590ce7adc083c0ed7c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (8007958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a3efc6783d934886d9905c35144b3edde805a1f6aadc4e6c520d174a9f1bae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:30:43 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:30:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:30:45 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:30:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bc8a4f20a4a5fcb0d7931643204ebba48c8b1b9d6e35cc8b7a43ed267c61a8`  
		Last Modified: Fri, 04 Nov 2022 23:31:19 GMT  
		Size: 5.2 MB (5200906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061571ab8afcf042cf8999f76ddd700b1f57e48dff2c7e8f0da290ac5870dbe`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e00ff4dd8efc7f40b28e5596b4244c34d719a2d58cec452a23b8e9102b36768`  
		Last Modified: Fri, 04 Nov 2022 23:31:18 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:0106bc0454bee2ffee13333551334ac2babc45d7a852191e2b81a2951ca62c24
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7577299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46413d3e55aa5bcfbb408a88741ddcc3c9acd32b847dc13c4eaf808bc6e1481c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:49:27 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:49:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:49:30 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:49:30 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:49:30 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ad00f67bd4d8a62c624d45cad5cf978dd5f4ae903a3fb20932cf8090437f05`  
		Last Modified: Fri, 04 Nov 2022 22:50:47 GMT  
		Size: 5.0 MB (4962359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b187b0997bad66a37052af0e653e1285af268b535a6013c71bad2c46d4c459`  
		Last Modified: Fri, 04 Nov 2022 22:50:45 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166265299c1efdd6832d07637383c6af588534bf0e7a13ccb2f4459277bc417b`  
		Last Modified: Fri, 04 Nov 2022 22:50:46 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:ea79710790666370759d3ac1f420876ed558153efe1f3aaf7e9b71755c0f2c81
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db5f8a88978775f76954b3994afba6c0caf852bfcbfea8dcfed4174582d5d0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 23:07:53 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:07:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 23:07:56 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 23:07:56 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 23:07:56 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebdfdc1026c56da7563e9e33db67d37ff822872d54ba452f0ae6077393460cf`  
		Last Modified: Fri, 04 Nov 2022 23:09:14 GMT  
		Size: 5.0 MB (4955790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76d8da00212aceef61792e206a3b5a9aac895414564457c350f6d3407a438f`  
		Last Modified: Fri, 04 Nov 2022 23:09:12 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb35877a4e69aec93d526917035fc480c866812832c17f6aebc407eb8d7a95f5`  
		Last Modified: Fri, 04 Nov 2022 23:09:13 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d94de164d5ae7db6570d21714bb57ebe3c9258aebbd286d5a9b42b754ea912ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7153d330b04656e57682588e1006c282b24ea413dc1383baa427260c39251f34`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 04 Nov 2022 22:48:05 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 22:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 04 Nov 2022 22:48:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 04 Nov 2022 22:48:08 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 04 Nov 2022 22:48:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25b40a25ec88a4c6fc9abdad0c94131f8e6f505dc968fa536626d7891cadb8`  
		Last Modified: Fri, 04 Nov 2022 22:48:41 GMT  
		Size: 4.8 MB (4786400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ea5272ea896a787b7fc4a6b58e843d8b642ad0a94926ae487ff817d09b35d5`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520c3dc887863f61ebd1ea5776203113e01a0aa6408784ce078cc0a20f06174`  
		Last Modified: Fri, 04 Nov 2022 22:48:40 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:194a8dab745155aa91ab7a025ec1b6462cd95ef1aef0c736b20fbb717c1defa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3532; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:nanoserver` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:285df485f8d2b409343b431afda5f6145cb9fc179ab79fdd2183bac4bf444540
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:c65d142974e6e7f5fe8384128cd8dbdb9b2668a1e4fb49aeeca4a3654b2f7438
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111746393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1781e373ba9536087e843a9f023257d774e6cce739d4ed55c2cb0d7f47e69950`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Tue, 11 Oct 2022 17:25:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:46:48 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:49 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:50 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:51 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9663157a1b8c7ebfc835c70cef562479a45950b091ce936a265a510fe6c647d`  
		Last Modified: Tue, 11 Oct 2022 17:26:55 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf887d12a075a1bf2182a64d525f363325e5725f2bc19e3af703f3beacd6f001`  
		Last Modified: Fri, 04 Nov 2022 23:47:45 GMT  
		Size: 5.0 MB (4966172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda7404e9d7755d6406fa6085ae959bc897d9d898146792212966553ca69fe70`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d449a0cf745bf57baaf8ee363c788258b610ad03cdca4f289b8b7ef3c8399ff`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb3650fc19510393e08f48559c3b7f76e30342c7e97545a04f46cc1137c8a80d`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fad28df4ca3277f7e21f347ee50418ffd6052365e935e67a8c7f790ceba61`  
		Last Modified: Fri, 04 Nov 2022 23:47:44 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:96bb5587358dc2025d7c44fa262b026bd159b99afa0f5c38221e9479230fea63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull nats@sha256:583a154f872d502770c0c1990662529b2e3ff025276f4616f8436a9886a5fbe0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2779177599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a74ba1b75336fd2776df351c7d5b58a594855ec7a7dd96c019aae0d85abda4`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 17:22:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 11 Oct 2022 17:22:08 GMT
ENV NATS_DOCKERIZED=1
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER=2.9.6
# Fri, 04 Nov 2022 23:43:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Fri, 04 Nov 2022 23:43:34 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Fri, 04 Nov 2022 23:44:40 GMT
RUN Set-PSDebug -Trace 2
# Fri, 04 Nov 2022 23:46:34 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 04 Nov 2022 23:46:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 04 Nov 2022 23:46:36 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:46:37 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 04 Nov 2022 23:46:38 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6193ab94a0498ba6454e2a35e189837b37a2eb01403e8b62654bdc28a4569c`  
		Last Modified: Mon, 17 Oct 2022 21:52:22 GMT  
		Size: 849.2 MB (849228999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c778a0131ae2f1653f1fb703f05998e74365629f70b1a15a0360fb1292182846`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ce79ce85e7eb7d4b12316d81cc8cb3ff2567ee214f4aa0bbf36933fd55891f`  
		Last Modified: Tue, 11 Oct 2022 17:26:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8f2b42cc55a80066c40803248bcd944b2e9d91b4816cd3ce1d28b443d73f00`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ba1db14d0368dc5a8550d542ceb29b2547b7dbed75d58bf1b487ea304f4833`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c39058dc1a861d07eb7c76cea4f1453df1c80785e1cd73a57b1cbe54b539e6`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48988848fc3aac57c4657605637681d89e28c7fb6f4111cce0269c7161baf9db`  
		Last Modified: Fri, 04 Nov 2022 23:47:27 GMT  
		Size: 357.9 KB (357949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7043fb33d1c6723cd7d2cd093a39eab66e7d100676ffef06a2bd07a2f6332fbf`  
		Last Modified: Fri, 04 Nov 2022 23:47:26 GMT  
		Size: 5.3 MB (5307986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2dd5ad15cea0202d17fcc0b2a77ce04a4d6ad74b0b3dcd5163365f9e9bbfa9`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaab41075f644d9851a05a34bc468748e87ee0e266027f90f6b5fd21d6a912ca`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91f95f5391a04697266fedd3f9bfa77d45b13155eea7c56c89a956ae2fecd88`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c5b9e0ee0274c8e0f8c62e405c6ea9629b10afd27bf4663f0eb9be31e996f`  
		Last Modified: Fri, 04 Nov 2022 23:47:25 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
