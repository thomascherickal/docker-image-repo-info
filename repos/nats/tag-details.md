<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.15`](#nats2-alpine315)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.8`](#nats28)
-	[`nats:2.8-alpine`](#nats28-alpine)
-	[`nats:2.8-alpine3.15`](#nats28-alpine315)
-	[`nats:2.8-linux`](#nats28-linux)
-	[`nats:2.8-nanoserver`](#nats28-nanoserver)
-	[`nats:2.8-nanoserver-1809`](#nats28-nanoserver-1809)
-	[`nats:2.8-scratch`](#nats28-scratch)
-	[`nats:2.8-windowsservercore`](#nats28-windowsservercore)
-	[`nats:2.8-windowsservercore-1809`](#nats28-windowsservercore-1809)
-	[`nats:2.8.4`](#nats284)
-	[`nats:2.8.4-alpine`](#nats284-alpine)
-	[`nats:2.8.4-alpine3.15`](#nats284-alpine315)
-	[`nats:2.8.4-linux`](#nats284-linux)
-	[`nats:2.8.4-nanoserver`](#nats284-nanoserver)
-	[`nats:2.8.4-nanoserver-1809`](#nats284-nanoserver-1809)
-	[`nats:2.8.4-scratch`](#nats284-scratch)
-	[`nats:2.8.4-windowsservercore`](#nats284-windowsservercore)
-	[`nats:2.8.4-windowsservercore-1809`](#nats284-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.15`](#natsalpine315)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:4ee342fdd2293351b2e2022a745aea1d21e7e09255a54cfc08c7511ef5026d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3165; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

```console
$ docker pull nats@sha256:4ee342fdd2293351b2e2022a745aea1d21e7e09255a54cfc08c7511ef5026d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine3.15`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-linux`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver-1809`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-scratch`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4`

```console
$ docker pull nats@sha256:4ee342fdd2293351b2e2022a745aea1d21e7e09255a54cfc08c7511ef5026d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8.4` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-alpine`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-alpine3.15`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-linux`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-nanoserver`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8.4-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-nanoserver-1809`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8.4-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-scratch`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-windowsservercore`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8.4-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:2.8.4-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:20f7dde8d076648302a894d16b5d432d42c436fc058abe0e55e723f17013ecd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2fd61199055f4c36caf283625d1ad6cd750b6d88381beaeff2861461d28d8dc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7680125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96919bfb87525e70a8bf5a6f9b59cabac00c6c3e12c050a5d8de8f257b70134d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:42:17 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 03:42:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 03:42:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 03:42:19 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 03:42:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:42:19 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ad4182d2d5a0fb34b282b1b978bd7e3993148de0338dc23fa32bec95e816bd`  
		Last Modified: Wed, 20 Jul 2022 03:42:53 GMT  
		Size: 4.9 MB (4864482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f390e783356445c282da30facfe33f33d632e28cdd738727055be1b6ac105`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fd4e7a11a952043e7ec2c8b11dc4fc2d05905108640ed0dba9cd98857fc686`  
		Last Modified: Wed, 20 Jul 2022 03:42:52 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:ce1a0d5feba1dea7b75d42a2cf9f0db37008aa23611208f0636d2e854f3e4e39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787a0f7c8f446c6de7f76a546e1b7816713946ff4446c8b8ab3300a076b84ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:34:53 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 04:34:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 04:34:57 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 04:34:58 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 04:34:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:34:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d8cdff31cbcbff5a77bad319304be00f6bfee5e7a0b3e79bb5098a172211b1`  
		Last Modified: Wed, 20 Jul 2022 04:37:01 GMT  
		Size: 4.5 MB (4518598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f94963426fbd74891e24cad2378e102449638365b7c4d30dea2b2a42afa3964`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6849175061bf5248fac59f399e2663721962abef73263e1e4055ef7d1878e6`  
		Last Modified: Wed, 20 Jul 2022 04:36:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:f226954f13c1edd6395e9cc413637020af72480481ab4d8fcc5627081dcf23b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e057b04bf0abc4d2d963120b94fed1ec0e43db4d5e28d9c0bde6d03b0e482165`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 10:25:38 GMT
ENV NATS_SERVER=2.8.4
# Wed, 20 Jul 2022 10:25:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 20 Jul 2022 10:25:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 20 Jul 2022 10:25:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 20 Jul 2022 10:25:43 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Jul 2022 10:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 10:25:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d3b1b592d1330908ca38e00657341d8084800d6e7a2e13ca39af6355c6bdb8`  
		Last Modified: Wed, 20 Jul 2022 10:27:51 GMT  
		Size: 4.5 MB (4513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ea8df768f9a5412372e5e846e3044908daf554b64ef735045ddcf755437c9e`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328bad88f834945c8d199b0d54dc6fa54b668a9d7b01ca89ee611d83d47c866`  
		Last Modified: Wed, 20 Jul 2022 10:27:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1d7154e4491475ff8fb864a26874ba8b4b250864ad515419c96432134b79a03a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7234771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff14469067b8205c1030c0740c47b13a4cd70a4cb3cd3e3f02472b056353df3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:52:27 GMT
ENV NATS_SERVER=2.8.4
# Tue, 09 Aug 2022 20:52:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='75a53e10c640c8348bafe43300785d5147c91f60cd721c21ec896bc50727270a' ;; 		armhf) natsArch='arm6'; sha256='993a0d02ff9d0c74be31dc9e7ac1066659637c4897cc94ced2e0dc982fb428f3' ;; 		armv7) natsArch='arm7'; sha256='89e4191a0bc15c2196f2e6c1b2a3c4200576f6e8ec1176060b2a191c5e588b0d' ;; 		x86_64) natsArch='amd64'; sha256='da8c999ab0da5881fde68cba55238748d7310f28022fb78b9c07b420572a4b45' ;; 		x86) natsArch='386'; sha256='e94e5ec1076122e782527f4a98937c60c9eed4d04c6ba0364986cc58cd3ff8f8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 09 Aug 2022 20:52:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 09 Aug 2022 20:52:32 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 09 Aug 2022 20:52:32 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 20:52:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:52:34 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0beb1bc3611827acd1326750497c2cc98b9160ed5aec13a1112ad88b6ba136`  
		Last Modified: Tue, 09 Aug 2022 20:53:33 GMT  
		Size: 4.5 MB (4515360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20f9bb5cbf9bb42bf80058089fa2cc11fe7eaad0e4342ef69340f9421360e9`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b065ba618e0c23dec2ae44bb9555ee098a0827cf44bc5f30ae1d9448e11f668`  
		Last Modified: Tue, 09 Aug 2022 20:53:31 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:4ee342fdd2293351b2e2022a745aea1d21e7e09255a54cfc08c7511ef5026d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3165; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:dfafa893be87c7c43364753241394c8e01cbf6480b2c1bd7ec1f91ab5fe1b67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:f2a38c4447751f62a883179308424a9ee332d1ebb94aece698645248426a4f04
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107794699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e08456814f3953c5161a388af2d43596a8cfa278b3a2cf347e44175f35ad55`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:43:20 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:43:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:23 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:24 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:426914f8f9a4bf93afd51c902139b25ee4faa60707c7fe5f889f66f8f73c9078`  
		Last Modified: Wed, 13 Jul 2022 14:44:16 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bb648acfd9f470692181b6dbab5d1b00e1a457d3c0f6b3559948b3bd385adc`  
		Last Modified: Wed, 13 Jul 2022 14:44:14 GMT  
		Size: 4.6 MB (4633251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a56c864b3b6433e8e122278da989fbc1a7cf1f1d015f71944f775074795d23`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d128925ba6db05c1bc268cf09f54964ae9a2bb68c3903b6ab7a0dbf3369ea84`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1553111043a7934df7e54c2a3d638b13a097b0bac727754535b3aaaec446bc6e`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c3ef780e824376c34040672637b1a9ba280178d48ec4f42d75aea632c85312`  
		Last Modified: Wed, 13 Jul 2022 14:44:13 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:6e96b99197f9d66e34df638ca22426d21963c643bfd0c987b45f1aecb814bc8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7df9a2712c9b7e57f228a270f9fdfaf95f8662890dd90719ab08952fe93cc99d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92a86f50672b8fb25a83d599295659904a27d366e8cad89089ddb9171c79e31c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:56:05 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 26 May 2022 23:56:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:56:05 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:56:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:56:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:56:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80ba54887e3752f04df58e1ab68c9805dc2aee54c543d487d8d51a2c88afc1`  
		Last Modified: Thu, 26 May 2022 23:58:18 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:208577394199773ff99d68d668bf4830314a173d7de8407e2bc5666b1d6d4a34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96128257f8f2facb4a2f726619b86453544d9108ec209c3665ec78c2dd14acf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Fri, 27 May 2022 00:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:25:52 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:25:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:25:53 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:25:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1306305db51c19253939f28312d2e4a694eab31b920aeef7d9a4d0a0b76f045`  
		Last Modified: Fri, 27 May 2022 00:28:13 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:2185d34a08baa2254fffd6480037c66a2091c564c7c652441d163e7e473602c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull nats@sha256:dfae260da4b1b30f0dbe480efc2a7811aa71287765113302c555247a3573c322
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2677363569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af592cb0901893fba48dabeba84c806d1b70791a6751af63a243ee95330b9331`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Wed, 13 Jul 2022 12:49:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Jul 2022 14:40:53 GMT
ENV NATS_DOCKERIZED=1
# Wed, 13 Jul 2022 14:40:54 GMT
ENV NATS_SERVER=2.8.4
# Wed, 13 Jul 2022 14:40:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.4/nats-server-v2.8.4-windows-amd64.zip
# Wed, 13 Jul 2022 14:40:56 GMT
ENV NATS_SERVER_SHASUM=911e8b77cf288c6e0997891d1400e5cc59dedd928e8f1685650c468674b52dc8
# Wed, 13 Jul 2022 14:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 13 Jul 2022 14:43:09 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 13 Jul 2022 14:43:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 13 Jul 2022 14:43:11 GMT
EXPOSE 4222 6222 8222
# Wed, 13 Jul 2022 14:43:12 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 13 Jul 2022 14:43:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:49b5d162039eae4fe1f7d6cc0d4b3be061cabb5d1d89950262e1b010e7ed67bb`  
		Last Modified: Wed, 13 Jul 2022 14:16:59 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a2b176476aa48539273d15d106f9687175e98ae9c9a718eb29874b4890126f`  
		Last Modified: Wed, 13 Jul 2022 14:43:57 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9ea1caa02772da0597ba779df4ccc227978e1dd60feb4064aa66d118e788`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b777f37e586af68c6b7df1d868b3e856fff928314a916dbb1199cd57bf0baa56`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f47e5948a3f7df42d74974a6a5becdfe5e98587748a520668a761351153f7`  
		Last Modified: Wed, 13 Jul 2022 14:43:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81cbc2b52ad93c44ea5782e539d9528b4b8371bcaeefe8d4094d95bc246b50`  
		Last Modified: Wed, 13 Jul 2022 14:43:55 GMT  
		Size: 346.8 KB (346783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a0d8e174ea86f326ba4fce1dbb8e0a458b0d006989ddcb7d641b8d77ab6131`  
		Last Modified: Wed, 13 Jul 2022 14:43:54 GMT  
		Size: 5.0 MB (4959739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8704d324de2c24ce52625e9df560ccb9f70dfa158e83cc7bb84133556ef0c065`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8409bdc3daa3e5113f112cf6bdf585a4eb047a256982287a6b2f531b14c052`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32141d3830a2fab08c09cc3863d9627edac56d0c774016ad84e87b8f98d446ca`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f022b00180c3ed89168447954f3e80c281a7c8a79964a6dbe5f894c2fcfba88`  
		Last Modified: Wed, 13 Jul 2022 14:43:53 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
