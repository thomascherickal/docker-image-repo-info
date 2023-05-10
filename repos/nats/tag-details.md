<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.17`](#nats2-alpine317)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.17`](#nats29-alpine317)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.16`](#nats2916)
-	[`nats:2.9.16-alpine`](#nats2916-alpine)
-	[`nats:2.9.16-alpine3.17`](#nats2916-alpine317)
-	[`nats:2.9.16-linux`](#nats2916-linux)
-	[`nats:2.9.16-nanoserver`](#nats2916-nanoserver)
-	[`nats:2.9.16-nanoserver-1809`](#nats2916-nanoserver-1809)
-	[`nats:2.9.16-scratch`](#nats2916-scratch)
-	[`nats:2.9.16-windowsservercore`](#nats2916-windowsservercore)
-	[`nats:2.9.16-windowsservercore-1809`](#nats2916-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.17`](#natsalpine317)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:55fff46807f17c8e3ce521fa00e0b2b995fa4f456f7b5199cef121d52e3f3bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.17`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:55fff46807f17c8e3ce521fa00e0b2b995fa4f456f7b5199cef121d52e3f3bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.17`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16`

```console
$ docker pull nats@sha256:55fff46807f17c8e3ce521fa00e0b2b995fa4f456f7b5199cef121d52e3f3bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.16` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-alpine`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.16-alpine` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-alpine3.17`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.16-alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-linux`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.16-linux` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-nanoserver`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.16-nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-nanoserver-1809`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.16-nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-scratch`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.16-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.16-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-windowsservercore`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.16-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.16-windowsservercore-1809`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:2.9.16-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.17`

```console
$ docker pull nats@sha256:887f0193c5b72b66ff4795b807f3e9e324c34ffafbce612e54b2be8140a06de1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.17` - linux; amd64

```console
$ docker pull nats@sha256:4cf8af50005318d7ae2007591c1e9bd1ac7f902b0f356dec91430efd0ef8c994
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8682788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:657fde4007c4b6834917360e99c6d1d2aba8008f86063236cf1fafb1ac022404`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:24:45 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:24:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:24:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:24:48 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:24:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a72768d864179b39d8c07884fe7459cf29f17c02a2da5d2d5a003e1d0d098`  
		Last Modified: Mon, 17 Apr 2023 19:25:20 GMT  
		Size: 5.3 MB (5307226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:befe8af95517b5393870f754b0c98731cd944cb3bc6388ad633b656b1b895713`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6547dbd8ded3b9905491ab0a9c5494d6d71269e65e375a39d9054cb026db18`  
		Last Modified: Mon, 17 Apr 2023 19:25:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v6

```console
$ docker pull nats@sha256:746771ee513ee499510af00c3a9015f3be6ff8d47b1518486d64fedaca45720c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8185529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8da6fe87ff77cefdd120f95dc130435acf493deec5453446ca847ab5b230b1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:49:18 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc938d5206598495cef1feb630c43c86b92d0d3ea866edf955f4a1eacb41162`  
		Last Modified: Mon, 17 Apr 2023 19:49:45 GMT  
		Size: 5.1 MB (5073724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ea8310e497182461c8dea03fba4fdde4ae9223041c71da081b214038d3af97`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981be0f799e39abee41bab3c79dd3fbf03dd34d8922e9bbbc3845fadfb6736aa`  
		Last Modified: Mon, 17 Apr 2023 19:49:44 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm variant v7

```console
$ docker pull nats@sha256:5e672f55186edb38fbcb316bc445cb4f45b0e54e2fc8c5ed407b6c1d106c3013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7933002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fc05222015b47b2e00325c3e5978ec515d8f97c6690d4f34f609432a052985`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 20:15:13 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 20:15:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 20:15:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 20:15:15 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 20:15:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a8982047f1eac1437be4d49481ec4098e0432b9521dc5cfcfdd08bac121bc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:51 GMT  
		Size: 5.1 MB (5063482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e104e904df676b258d3fd91b2e207fc0237168b05041c5e1f3e455036acadbc2`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18169ea10be1f5bd1def88dda826c6c9ecbfedb230889c731af11e702391d1b`  
		Last Modified: Mon, 17 Apr 2023 20:15:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.17` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:7be5cb7858e2d42d45a85a57a4c7bdb1c667c5b4bf9336f256ff04d498a86abd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8149081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b26e3bb39c9cc89b55f133fcdcaad6954229b568545735bd4eb0ec1a06368b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Mon, 17 Apr 2023 19:39:57 GMT
ENV NATS_SERVER=2.9.16
# Mon, 17 Apr 2023 19:39:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f73c99954263dc49374e755028c3702b03656b64e3a2bb247d95a3c27bd02d27' ;; 		armhf) natsArch='arm6'; sha256='75726892cc2c852bf54bf3ff1761d6be6ff106e85e77452b7854e7dcc3c878bc' ;; 		armv7) natsArch='arm7'; sha256='28b965758b25412ac0307c4dbc394b2f6783035bf070521f3cfef1441b655b98' ;; 		x86_64) natsArch='amd64'; sha256='180b7f5f152733f9be1fcb0be607303a62c30b3e0d17bf2418fd548cd5c929df' ;; 		x86) natsArch='386'; sha256='16344af0854c89e51f1b0ac1ebdea85d03d52e6f47dcfe0297a88861bcbf211f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 17 Apr 2023 19:39:59 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 17 Apr 2023 19:40:00 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 17 Apr 2023 19:40:00 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 17 Apr 2023 19:40:00 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f65fb7a838c5934cc32ea5b7793d67da4be3517f31f6972c153a4625975c6`  
		Last Modified: Mon, 17 Apr 2023 19:40:38 GMT  
		Size: 4.9 MB (4886224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c74ba516d6f88a9d7c7154519a05593100f98e162483571ffd6389eaa52a69c`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8f146e84da60570288a587767bd992195d3b56ea09b2c211a25650cc98c29`  
		Last Modified: Mon, 17 Apr 2023 19:40:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:55fff46807f17c8e3ce521fa00e0b2b995fa4f456f7b5199cef121d52e3f3bc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4377; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:nanoserver` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:1507f0f2963897740a12da7508fd1bc6ebea7ebdad76eb111d235fb15a1a7f91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:6b63ca13550920e16ac8d1d383dc58df9d072c4c3fd4e511281d202dbe38c0bc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109468515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4679dd016bef3c8ed79c3b2d31d2c63a3476cd23995815bd0f30f6861672beef`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 May 2023 11:29:01 GMT
RUN Apply image 10.0.17763.4377
# Wed, 10 May 2023 02:43:57 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:097c54a43536c2c00c5d7ab4ca42531dfa5623331b43597ffed4871d2f7f7d72 in C:\nats-server.exe 
# Wed, 10 May 2023 02:43:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:44:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:44:02 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:44:03 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f7885e3a2dfeae5eea125d00da688c29930a05e4d904884fe43e093ce6223664`  
		Last Modified: Wed, 10 May 2023 01:49:01 GMT  
		Size: 104.4 MB (104383998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9af27dd7e62b7d94fa31a7c9efd9a532c42db89ec01fdb7fe430043ceabc5b4`  
		Last Modified: Wed, 10 May 2023 02:49:27 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d85a51b6ad0c0fa41d8acd3c2343413b08e446c0e8285547dc0f823bc8c79f`  
		Last Modified: Wed, 10 May 2023 07:09:52 GMT  
		Size: 5.1 MB (5078084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52698a3efa93904b0f9e31143300d218ee09e1094c4750deee936722a434c9f0`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354b5f484857495c910fe4f837972933f33fd6843557455f4bdf4f353ef6128f`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c06258e4387dc50c2c887507689557c15c1676fa0c66e537b7d0dd4d052267`  
		Last Modified: Wed, 10 May 2023 07:09:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1975391c3359e794cc1f15388c47f08ef7f9587a8f1ba4cf78d70a6586eaafd6`  
		Last Modified: Wed, 10 May 2023 07:09:50 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:1371882eca0a6f0d10d63254b47ebf60f1ce8e5bd625ec6c6ca2f629bd2a6bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:ae9aaacfe0a1ce4d691fe69df2fc9f816c832fe76c9968d82a81c8ea9bf8dee6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c01b1d61830e3fffe517a0e45b9024e8e5047f740c6422485687004dbecc9f5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:421063e5765f1083878517f41f0c32173cc7ed9577c58881bf9f2f7a13a00e63 in /nats-server 
# Mon, 17 Apr 2023 19:24:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:24:55 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:24:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:24:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:24:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:79bf10b6d07ffa612bdbc8ed452d38520187499b0b74471057fc4ffe0a5572db`  
		Last Modified: Mon, 17 Apr 2023 19:25:45 GMT  
		Size: 5.0 MB (5021619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc21c2bb595ab39591f5dd240f2a4bdb2f0b82a55b622281b9251646d58f9c`  
		Last Modified: Mon, 17 Apr 2023 19:25:44 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:831fc0e7fca982522287ddab3222ab3e6ac3110877308f67e8c08f15d84ea6b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4783467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d67f57dc16931f2dc4fe6408f89962b498acc075d5f8285b5fd359de9717cf9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:b90e99fa3478613cf230efdcdcf94e500fa9b94e3c7cefce53a8d75915969123 in /nats-server 
# Mon, 17 Apr 2023 19:49:28 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:49:28 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:49:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:49:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07bd219461ba5eefd9d4f65c3531742f2b23a5f9afbaa72aa9504df05e55d681`  
		Last Modified: Mon, 17 Apr 2023 19:50:07 GMT  
		Size: 4.8 MB (4782960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a6cb043f66c7e45dc5dc1159516f31dd7283d368cb45d9ace3ea71c7e13c7f`  
		Last Modified: Mon, 17 Apr 2023 19:50:06 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:d572537c0c0f4ad41f180a1ba368d24de7737ee2f04b326e52dd5b49a8b8a528
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4779539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55460692736f4113aef74dbc8e8a304e95a3c60f7a760d76b08acd7ffb192513`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:932d2dc410b9b0174a24a33b2a794befb8d31ee83b67b4650d54cf92198c9bb1 in /nats-server 
# Mon, 17 Apr 2023 20:15:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 20:15:32 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 20:15:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 20:15:32 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 20:15:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e820d218dd5a768c0a585da00fe0f7216f5fb7c61645b587fe5568aa73fa71f2`  
		Last Modified: Mon, 17 Apr 2023 20:16:11 GMT  
		Size: 4.8 MB (4779031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7e0fa1bc6892f90e7c6e7261a36ab5a8cdf352a585b683f0c0d1d1d3b80684`  
		Last Modified: Mon, 17 Apr 2023 20:16:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:55524640145ef26e3d332d1f42dedb4a350fc5dbbd7f7736afa9b9d8f5b8a52c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:454ed91868a5f8cd8b9cfe3436552b65dae93d04c2b33c5d944a61f319f862b0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:fbbc864e8ee6530cd73cf22189859d34083a1aad75ce26ab24d5c644538e897e in /nats-server 
# Mon, 17 Apr 2023 19:40:20 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 17 Apr 2023 19:40:20 GMT
EXPOSE 4222 6222 8222
# Mon, 17 Apr 2023 19:40:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 17 Apr 2023 19:40:20 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 17 Apr 2023 19:40:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5328b7e5868f05e8a85884ab403d6becd1f7d5bad74fbe6b2fab13c3021a81f5`  
		Last Modified: Mon, 17 Apr 2023 19:40:57 GMT  
		Size: 4.6 MB (4598800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c27d275a8e44f1e05ee9e9d85c6349edff3da332fee2ad77f6caca8526df3d`  
		Last Modified: Mon, 17 Apr 2023 19:40:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:f7cb4ed36f2be5c7be9a7b08d8c1b22e645f58ba4991dfa459e74577d9f4b615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull nats@sha256:1732bbcb34375aafeac01e77ce6e7aa2dbba27278ba12958bb3aed917f0c1dc0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2077822911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb2ac53edf941120e941b4913e75121f8f7849d6c69cd234724ac1354311`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 01:56:29 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 May 2023 02:40:26 GMT
ENV NATS_DOCKERIZED=1
# Wed, 10 May 2023 02:40:27 GMT
ENV NATS_SERVER=2.9.16
# Wed, 10 May 2023 02:40:28 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.16/nats-server-v2.9.16-windows-amd64.zip
# Wed, 10 May 2023 02:40:29 GMT
ENV NATS_SERVER_SHASUM=293013cd810f35f2a3dd25b0d850da248bc45af46b854a805383f848db3e9fa0
# Wed, 10 May 2023 02:41:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 10 May 2023 02:43:41 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 10 May 2023 02:43:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 May 2023 02:43:43 GMT
EXPOSE 4222 6222 8222
# Wed, 10 May 2023 02:43:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 May 2023 02:43:44 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a89be60a77cd8d520ec5f03d703ddbc15675dd1df4d95e041032cf08960af5`  
		Last Modified: Wed, 10 May 2023 02:23:36 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446cee93ab2781cfc08e135a3a7ab166e5342ee6817c34fb47e0662c085bbc29`  
		Last Modified: Wed, 10 May 2023 02:49:15 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de33925544fc248e0ffac22a06e9727c7ba90ba2cb7db16eeaaff706776402b`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135feb8500e9833370ec21c3622cf7fbba7424afcac727b61e304376265d4be`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5271c6f8ccb837e1ce744ad44305a94c606b0be8b8485718313913c90315cd`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bcd42cac1942260a2fe8430628f8d0f792cc8361dd67fab848150d01b97657`  
		Last Modified: Wed, 10 May 2023 07:09:36 GMT  
		Size: 426.3 KB (426266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a398f7862050ef8d8f732aef1986f5db3a45557b30ba2a17c22f482c023b9f`  
		Last Modified: Wed, 10 May 2023 07:09:35 GMT  
		Size: 5.3 MB (5348225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d534b19d5fbf3dd2d41d8086faca3ddedf186adbb103979e6d76101e3eec78d`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fd8189adda36aa8738fc9e85d0a25701a5a0e38a451afa5af1700e7e79d67e`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78173f06e168d48cc7aa1d4654204d98d914ae854728a118131ffe8d9181a82f`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd778f6318ee8c3823680bf429cf481faec2f6f7e714cde79309dfc917345a`  
		Last Modified: Wed, 10 May 2023 07:09:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
