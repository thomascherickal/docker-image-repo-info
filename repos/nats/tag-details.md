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
$ docker pull nats@sha256:9873de04d4fc85af649a69dc9f9fa6d93f35b320d115706722e0b4b278175919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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

### `nats:2` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.16`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:9873de04d4fc85af649a69dc9f9fa6d93f35b320d115706722e0b4b278175919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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

### `nats:2.9` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.16`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6`

```console
$ docker pull nats@sha256:9873de04d4fc85af649a69dc9f9fa6d93f35b320d115706722e0b4b278175919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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

### `nats:2.9.6` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-alpine`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-alpine3.16`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.6-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
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
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.6-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-nanoserver-1809`

```console
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.6-nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.6-windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.6-windowsservercore-1809`

```console
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:2.9.6-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.16`

```console
$ docker pull nats@sha256:ba1d3d9564004a89ee20c34f019afcd3683d3221c80602ec95d02e05de5b0aa3
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
$ docker pull nats@sha256:aa38aa991628755bb8f27826f3b5688534f871a528f92da8fd5060cdb62ab2c0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7578489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1113f11e09a3840e904549f317a6edc3242bbe3242accbe013893bd63b32342`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:33:56 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:33:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:33:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:33:59 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:33:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:33:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad55ca795a2109e29efe113d38cf5be22960dc5d72cd19f2deceff57c63a987`  
		Last Modified: Sat, 12 Nov 2022 04:35:17 GMT  
		Size: 5.0 MB (4962411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3247b15bed3a4ef31a4163c2d0311131d89ee6e01b7d331462d04b3d916b5260`  
		Last Modified: Sat, 12 Nov 2022 04:35:16 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c487b70d4a43929abb58108b5b9986c238bfc6980a9fb7ef7a56b5f2a93e375e`  
		Last Modified: Sat, 12 Nov 2022 04:35:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:9d1bbd448681d703ae510eb6c66dd1b52caf6c36cf08c60a23e9c9e394fdb172
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7373822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ab836153e13c3b80d353fdb184e2aa87ca3941b1e99c723fe5bc5a7fbb7baff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 10 Nov 2022 19:57:31 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Thu, 10 Nov 2022 19:57:31 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:15:38 GMT
ENV NATS_SERVER=2.9.6
# Fri, 11 Nov 2022 07:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 11 Nov 2022 07:15:41 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 11 Nov 2022 07:15:41 GMT
EXPOSE 4222 6222 8222
# Fri, 11 Nov 2022 07:15:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 07:15:42 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f95c291632d48fb04d9cab8d57481a5abad1904dc3a50688ec8f58978d50dba`  
		Last Modified: Fri, 11 Nov 2022 07:17:02 GMT  
		Size: 5.0 MB (4955786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed88c6a29511fb518b9e2a560419f0f105a425785049f1ba3b57cf7f3dcf6c63`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a778afa5e25157008d7402637f36cfa4f216f2a5f72e87b7848744a0f40f23`  
		Last Modified: Fri, 11 Nov 2022 07:17:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:43063296b032bac846846e4e3dd9208c526aff3b7e3790e66fc18632d764d857
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7495243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1f0a1d44d037ccd570d9d7f6ac6a89d12392ecbd6230a4b767d8a6e55b0322`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:30:54 GMT
ENV NATS_SERVER=2.9.6
# Sat, 12 Nov 2022 04:30:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='63574476145d3b73d20266e96d843a620e9fa57989b0841fd724df6ef39fcf9b' ;; 		armhf) natsArch='arm6'; sha256='77333e02d84c95d011c2a4125fc36b581c6314ebe1875ef68855200f750a2615' ;; 		armv7) natsArch='arm7'; sha256='bb39615307707c017d310387f05909e0495e803ae26da953a343d798562fa59b' ;; 		x86_64) natsArch='amd64'; sha256='847ca46d71044a87c360f3267b1bcfaef7b003ebd56221e728c1122b8be8c756' ;; 		x86) natsArch='386'; sha256='81e4978131eba37ceaec6e923d6a0b2722174d4d0aa56a58535d4c979e79861d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Sat, 12 Nov 2022 04:30:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Sat, 12 Nov 2022 04:30:57 GMT
EXPOSE 4222 6222 8222
# Sat, 12 Nov 2022 04:30:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 04:30:57 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c28a3b58a9a32866a0ce5ae0ea96429876fc6e4ddff42f869ae8c90151d137c`  
		Last Modified: Sat, 12 Nov 2022 04:31:29 GMT  
		Size: 4.8 MB (4786484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7cc2d315ec804021165c91007f9bfc3eb67ec28702a59b91256ad2f4e2171d`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a730c28724eff608a152b178885c260fb3bd8dbfd37a226282552a3937384b8`  
		Last Modified: Sat, 12 Nov 2022 04:31:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:9873de04d4fc85af649a69dc9f9fa6d93f35b320d115706722e0b4b278175919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3650; amd64

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

### `nats:latest` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:932b08c0337317adcd663aa38e0a55a9803ee6cbcd53f7cf36001daaef8c3b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:f0bdc15be988edf64cf892a77450834881d2c6c7dc82b9360bc52593a5aa0b14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111696158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054fa16934ca677fce3a8b34c00ace05149796083e264482875fbda0d23f6539`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 16:47:43 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:47:45 GMT
RUN cmd /S /C #(nop) COPY file:27c13fdcb069e821fef4075dc66fcddee176451571e6aa7486ebfdb5261b3db9 in C:\nats-server.exe 
# Wed, 09 Nov 2022 16:47:46 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6708525607bc7a2985c6a423e6cb63d6175e3ad60d997873c4519fab371772fe`  
		Last Modified: Wed, 09 Nov 2022 16:48:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c0e5b167a89f47defc32fac57f29e7c72ef828ad873eacf2127253ca009e02`  
		Last Modified: Wed, 09 Nov 2022 16:48:41 GMT  
		Size: 5.0 MB (4966166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1ef6dd873b0efdf79c9de73a56c7d7cca2722957a6281b7f6e4aaa950572da`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842bada13c0156df30e6332066f30698a9f967235704e763789afe20fc24af89`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e63e1c547824ed6c1142b32ecab108bbf2784a0659016df96eb2f6b0f140e0`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ba3f3f63b4b7c99e24b6221604b2f59a22f2f3ce9109e5998c44ef5e7ab8ce`  
		Last Modified: Wed, 09 Nov 2022 16:48:40 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:3389f85e0e7409ff650a13c55949b8479f26722851ed67d7d729b916da30fd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull nats@sha256:e41754ef90643bf069cb84ea5f668b90d6e87d5dc893892365da862bcb8e6b28
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784261872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6657882ae13b4d8042bf2e2496662461c4bb3edfa1b13dd86573644fae02bdbc`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Wed, 09 Nov 2022 14:50:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Nov 2022 16:44:45 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER=2.9.6
# Wed, 09 Nov 2022 16:44:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.6/nats-server-v2.9.6-windows-amd64.zip
# Wed, 09 Nov 2022 16:44:47 GMT
ENV NATS_SERVER_SHASUM=1c627ca06ec40fafd26befac35640a6fefc63bbb16cbb594f74d493ba670f2c6
# Wed, 09 Nov 2022 16:45:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Nov 2022 16:47:25 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Nov 2022 16:47:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 09 Nov 2022 16:47:27 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Nov 2022 16:47:28 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Nov 2022 16:47:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99941fb33972e616b231a8aadd93463fdfd5de6aece4aa6c470d2feec31839be`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f3d8a87f0a1540850986ff94131286dfa42ca116f04779e02f60b3a724641b`  
		Last Modified: Wed, 09 Nov 2022 16:48:23 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23322c383be4156ea3e0f20a481efd18b9c3bc4985eb67c6f77d626d92e87bd5`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9284e4cc7c4758292b1e78f2080cd5df93d0d78a2bebe4c09346556272cf88e`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578f0b75bab1273f0521ef89bb563f4b3f525708b3ed846b038128137ca2487`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd0fa9993c097d11161a0eabac8e8e9ab7e0b7de142c1b50d2eda742ce7bf94`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 358.6 KB (358602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecb0068e158479db8e23a4f17e3d634187e5565fefc58fbd239fc79783be5a3`  
		Last Modified: Wed, 09 Nov 2022 16:48:21 GMT  
		Size: 5.3 MB (5303625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b232f78a915c29589007d3cb21b64cd7a5105eab2cf012f3f5611287941569`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5076e2a144a8448de3e2a434deeb71894af3f8f4fd439afd197788d7c990cda0`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed22c3b339e85309fe22a7e2079347d9ea486185119e911edbe6b1f6c4f60ac`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e163e46114b71691249b4d7125d6c2b2b41a5a48b185b28471f915ed2389226`  
		Last Modified: Wed, 09 Nov 2022 16:48:18 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
