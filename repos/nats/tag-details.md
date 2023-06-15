<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.18`](#nats2918)
-	[`nats:2.9.18-alpine`](#nats2918-alpine)
-	[`nats:2.9.18-alpine3.18`](#nats2918-alpine318)
-	[`nats:2.9.18-linux`](#nats2918-linux)
-	[`nats:2.9.18-nanoserver`](#nats2918-nanoserver)
-	[`nats:2.9.18-nanoserver-1809`](#nats2918-nanoserver-1809)
-	[`nats:2.9.18-scratch`](#nats2918-scratch)
-	[`nats:2.9.18-windowsservercore`](#nats2918-windowsservercore)
-	[`nats:2.9.18-windowsservercore-1809`](#nats2918-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:40d48cba5bed37f53983436599567d26d6840d6e9bc5d30f2e33041b8a38b20d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:40d48cba5bed37f53983436599567d26d6840d6e9bc5d30f2e33041b8a38b20d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18`

```console
$ docker pull nats@sha256:40d48cba5bed37f53983436599567d26d6840d6e9bc5d30f2e33041b8a38b20d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.18` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-alpine`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.18-alpine` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-alpine3.18`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.18-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-linux`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.18-linux` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-nanoserver`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.18-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-nanoserver-1809`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.18-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-scratch`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.18-scratch` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.18-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-windowsservercore`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.18-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.18-windowsservercore-1809`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:2.9.18-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:6c536d9063125318cd4141ec5e597dc83a0cae45f0d83af93f21b33e3e52158c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:152ca536212bf33db49cb71cfe8fb3f69847e56d32db267db65d76a5bcab4234
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8806931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a41da954f9c6f11bd01c6f06b952be226be4cec1abfd318541c99d551822b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:18:46 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 00:18:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 00:18:48 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 00:18:48 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 00:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:18:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4911ea1b2d2da5340d06d36297f2947c28b665c5532b5411102b01a3791da4f6`  
		Last Modified: Thu, 15 Jun 2023 00:19:24 GMT  
		Size: 5.4 MB (5408050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ebe95c01c1ec4327f35f0c0d2238000d8d16a1ef53e95243f8e2879448d4c0`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04507ea59681aa3784317a4cdb8a34a2e6ec1441e934ceba9a4ef9756335464d`  
		Last Modified: Thu, 15 Jun 2023 00:19:23 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6ce23adaa64ba1092093a4dd12d27530c371095de7ee80335cee7952317f4144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8314492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e2a8870d2bf594715bb364438d34fa6ebd58a288c9a32e0120e9f58a04a39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:11:22 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 20:11:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 20:11:26 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:11:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 20:11:27 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717d37d3b660cb6436a8e51489a17930f45b0ffb973ac265bf0e59a67a295d57`  
		Last Modified: Wed, 14 Jun 2023 20:11:54 GMT  
		Size: 5.2 MB (5170142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293a38d784e4b9606106edc939e280ad05445c4a6fa49d08654050eed8987bb8`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522499e8988ce8d2e7120f88759a6c30d8acf834c11f5e78fb4f36e3cc2df377`  
		Last Modified: Wed, 14 Jun 2023 20:11:53 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:5a6f96273b0961172f1dcbc5a75d26744674aa13bf8c76cf685392e03a8e8504
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8074659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78086fa95cc21fa070f0634500d489cb981c0dd640e15f9c031ebadf8950210d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 04:51:52 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 04:51:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Wed, 14 Jun 2023 04:51:54 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 14 Jun 2023 04:51:54 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:51:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 04:51:54 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59ab22b83a8145ddd2d19db95e3e93e0b5e10de697667ab1ec4ffc64b15edbf`  
		Last Modified: Wed, 14 Jun 2023 04:52:34 GMT  
		Size: 5.2 MB (5162544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48624584aa6515f3c410b3adec525f8eb6637d77ab49ea0721591ad0c39bc13`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eb0308bc7ad5233d699e43f31008d243b2199afe58aa39168d553a4f58f2fe`  
		Last Modified: Wed, 14 Jun 2023 04:52:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d475680f3e9e4332e6af79a95273492786458eca70261525fc6d564ba84910a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8301899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab03fece52e8856c77ceb8679f18b9cb272f007e92c4783aae54fe932025fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:03:33 GMT
ENV NATS_SERVER=2.9.18
# Thu, 15 Jun 2023 03:03:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='f5ea0ace65873cf81dde2951d9130f6ecad3f96e80a59badb259a66fc3294579' ;; 		armhf) natsArch='arm6'; sha256='f7dd549c09bac2adcc3260868bf5f182645c8e59e7b9cb868feff244017998b0' ;; 		armv7) natsArch='arm7'; sha256='bb1015887864e7eeeeb8bef4c9e06bd20d865b01a67bab8bab802ef5483bb6ad' ;; 		x86_64) natsArch='amd64'; sha256='c61c5dd662ed0836d752ed98508d5a7328d85e6126d2cf9784a0d546a64c961c' ;; 		x86) natsArch='386'; sha256='68467b7d83a96a554257b84464bdff34de956af93971e43faa711e1cb29249c8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 15 Jun 2023 03:03:35 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 15 Jun 2023 03:03:35 GMT
EXPOSE 4222 6222 8222
# Thu, 15 Jun 2023 03:03:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 03:03:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0843e2a14dc00489db58ce6379f8e6ad0cf49ae10cc1ddbb68451d4bef1fe74`  
		Last Modified: Thu, 15 Jun 2023 03:04:01 GMT  
		Size: 5.0 MB (4971647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7be6c5f72357ebb8eddacdf7a7f85658a445fc279e8cc51e980d9ead5408d55`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea43bedcc5329dd1083335ee3d93acc5a8879cde8ae704c1fc24e26092492623`  
		Last Modified: Thu, 15 Jun 2023 03:04:00 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:40d48cba5bed37f53983436599567d26d6840d6e9bc5d30f2e33041b8a38b20d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4499; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:3607b6c20043494b666fbfd2fea83b50b79470dadcdcb5a25332091eb0865ce7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:6e78b57a2010189c5b419130055b295f0b45ffd01d9d693e473a8b0455b04931
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109577889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f78f2040b93146d50e68bca77f438d15f51186b7b5d264c5aff87781bffe5ff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 20:19:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:e92fb324fb1e715aaa4f213ef42afe80c4a76690e3b2d439bee510cb2ae47cd5 in C:\nats-server.exe 
# Wed, 14 Jun 2023 20:19:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:19:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:19:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:19:07 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad82a63ae84196afc54c5956c7877278d6c0b6a91e47222a50d790c2d9e07f5e`  
		Last Modified: Wed, 14 Jun 2023 20:19:50 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa91c896c6fb45a9c5f783f062b792391b211d8d17964941c5352cf6858b2a5`  
		Last Modified: Wed, 14 Jun 2023 20:19:49 GMT  
		Size: 5.2 MB (5174009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5c072b8b934a1081d0260d8379c92eea084db8d38a9dd214b4ea3899a6e16b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6082349db6622caea203da789c29a17747b2739c95012aaa531888976e1201b`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ac5b8008f5ff928e6f1b971f089660417ed155b4f5a79843cf73a03e08a103`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0536d4c38572e98e3b7b614620d8ba6a0b1186e628f440e2d3aa9cc354d7e75a`  
		Last Modified: Wed, 14 Jun 2023 20:19:48 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:8f3e4bf5d848f0eaf248bfbc8249d53c1ef590b6da3f96ea4d723a05f2e4436d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:a745065ae9a8f32cc91b2071488c1f59436f5f37f34c7c6b8cc92151faa0e3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5122440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5890e892d1ad969919c44edd59234aba90bed05efa593466e4febb8894ffcdd0`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:b153b1503cf6a82c5cc80b44ddaff7ccc3405ac7d7709c9b40a9e173ba2f50f1 in /nats-server 
# Wed, 14 Jun 2023 04:35:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:35:22 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:35:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:35:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:35:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8b0c326d1b5e38f75b5b85a41c0a33b3dded3024fc094e69c586e8502027c3e3`  
		Last Modified: Wed, 14 Jun 2023 04:36:07 GMT  
		Size: 5.1 MB (5121932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7c6ae7a938b576ab8648f86530b510f2be9541d3822aa3378fc924927f2fbf`  
		Last Modified: Wed, 14 Jun 2023 04:36:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:f26f23aad2feedaeaca9df38eca5559b431fbb8ed841789b1e6b2c3c84ffa79b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae95e37599ef924cfe3d5890b3af209e09951179f6672d35af6811876e61253`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:e5bb5e8247a1c4bdb92d70dc84443f615728207816f4c76763893029e98fe987 in /nats-server 
# Tue, 13 Jun 2023 21:49:33 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 21:49:33 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 21:49:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 21:49:33 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 21:49:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7f1a7a7f3e313c163918678d53d48af6476087e63070356ad38ff1c041606bca`  
		Last Modified: Tue, 13 Jun 2023 21:50:13 GMT  
		Size: 4.9 MB (4884348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af05a149bcbd29ea7705539c8b49e2c00b5883848519f3929bf4c4dc424022e`  
		Last Modified: Tue, 13 Jun 2023 21:50:12 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:ddf36c6f5382250cf0c060174d558e0baa7f3476a02202f6f2c62704d8c2291f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f106a7db0d6aeb34de7f7373b5a9730cae54001f06148c1cd6009bf01bfa9f33`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:e75b1e12b729f292a57f2d1659447109dff58c1d8490e106b86376f59145089b in /nats-server 
# Wed, 14 Jun 2023 04:52:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 14 Jun 2023 04:52:17 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 04:52:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 14 Jun 2023 04:52:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 14 Jun 2023 04:52:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea8b2adaa2a72f51d0db4333759ca7e2991e083292d08571a49ee462a01d9068`  
		Last Modified: Wed, 14 Jun 2023 04:52:54 GMT  
		Size: 4.9 MB (4876001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9750ae1eb25bd2c63839e3ccde3cd9f97e8556cc9b72a65afa7463bd715448`  
		Last Modified: Wed, 14 Jun 2023 04:52:53 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:edbf69c3a8dab18af6eefffc70fcea84205a4397632e23fbde4cca5fe03446ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b395b40ae1ff951faa10f8f5c05810b77b0a03c2ef5a8eaa8bc443497b52348d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:0fec8537fba7c573dbe20b854a6b32d8b0940e46f9e81c41611d447b82a034bc in /nats-server 
# Tue, 13 Jun 2023 22:34:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 13 Jun 2023 22:34:13 GMT
EXPOSE 4222 6222 8222
# Tue, 13 Jun 2023 22:34:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 13 Jun 2023 22:34:14 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 13 Jun 2023 22:34:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:2cce796fcd5a4e60d6ca871c71b29485d80a6babd1c43a056db0b52aa6e904b6`  
		Last Modified: Tue, 13 Jun 2023 22:34:58 GMT  
		Size: 4.7 MB (4687516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22153c0efa275cbe62c344213d16db73c5732467534b2a316e379bdd77324d29`  
		Last Modified: Tue, 13 Jun 2023 22:34:57 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:22465402ce357b9bbbfaf3853dc904e34184d828edb472868673c38a02e6b7b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull nats@sha256:03f97fcd9cd3319e75ebb981c3af42c2a88b95e2f484ec3aeff1c1d734b063ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1656404940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c30b9773f8a110b38afb110496f37de9933ce5b90e82dd0a8f843b9ba35acae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 19:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jun 2023 20:17:19 GMT
ENV NATS_DOCKERIZED=1
# Wed, 14 Jun 2023 20:17:20 GMT
ENV NATS_SERVER=2.9.18
# Wed, 14 Jun 2023 20:17:21 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.18/nats-server-v2.9.18-windows-amd64.zip
# Wed, 14 Jun 2023 20:17:22 GMT
ENV NATS_SERVER_SHASUM=139c2d63193d7df39894b144fb08a40e15548f89087e1932617239d36ab0c901
# Wed, 14 Jun 2023 20:17:45 GMT
RUN Set-PSDebug -Trace 2
# Wed, 14 Jun 2023 20:18:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 14 Jun 2023 20:18:44 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 14 Jun 2023 20:18:45 GMT
EXPOSE 4222 6222 8222
# Wed, 14 Jun 2023 20:18:46 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 14 Jun 2023 20:18:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3929a070e5d6b9cb95587cf41492d8ef77aaa7e9f90fa3cd1b32619fae5debc2`  
		Last Modified: Wed, 14 Jun 2023 19:51:36 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc032b2e13168aa149afc2fa80f0046e2522b46496b0b11ae5e6e6cde6afec87`  
		Last Modified: Wed, 14 Jun 2023 20:19:35 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020d266b90663e4a08cb8a268fc54c8cb1a9241c336a6e6f1729e16f0d135e3`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c30d3a997645f33d20fa13eac290bff874dafd9baba7e27c28a05e7d632da18`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6755ab33ed91c39427a9de6eabcccda0b4c01d801297a953d3c40fc83068615a`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7048ba31253f6a437a2d43c565b8623badd9ae698c3ea2bf3943ee00766b4e8`  
		Last Modified: Wed, 14 Jun 2023 20:19:33 GMT  
		Size: 312.2 KB (312236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30a85805c362c48c21ea4be8fc389308321d19232ae7d53303327a8555a8c84`  
		Last Modified: Wed, 14 Jun 2023 20:19:32 GMT  
		Size: 5.5 MB (5459741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcfa853498f5e05ae2c6947a076308947a387e316039424fc1f12d648e8a0`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb7e8f0d98fec70cae8dba259447711fa6d4b0fdb1762b2b9a2344a07731c6`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d1c9c860ba23fd419460f5b0eff7bd724ccee531b796c44310f67d24a8ac6c`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e308156f464715dfbae62b48af7822328ee169a1c20a534a5a622ef9bbb1ce`  
		Last Modified: Wed, 14 Jun 2023 20:19:31 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
