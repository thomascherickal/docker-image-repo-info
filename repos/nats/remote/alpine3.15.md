## `nats:alpine3.15`

```console
$ docker pull nats@sha256:5c9586bb97675d0a82284e1c13a88126b4931ddd2fe67d652f06a00ead649a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:911802abf8c7fe0e6a087b1dd6cda8e2672cb54a0f378a8a9ec392154c2874cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7666004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3aec2c460095775d7c33564e0d17602499e234643ecd340a19d96f1ed659f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:06:01 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:06:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:06:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:06:03 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:06:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:06:03 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e611d6827355a555e7444f59b1ded7287dd52b0bbfe386b26ec29c93e5512438`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 4.9 MB (4850448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71ea3c76b52c4f5defd453f3c496042d7b4a3d2bbf6e288dfa5af05cd46bfe6`  
		Last Modified: Tue, 19 Apr 2022 03:06:33 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eceee0c6c7dacc7589e2863a176124de6f67fbfa21a92791b90316381098f307`  
		Last Modified: Tue, 19 Apr 2022 03:06:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:2ae53b791ab630e2f8f43d6d508c9c8ae82edde3cefd2c5c400b30d81f3db1c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7132372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c353e09461884a12dabef76baa7680026551e6201af4617cffcff367b02dd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 01:55:10 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 01:55:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 01:55:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 01:55:15 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 01:55:15 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 01:55:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 01:55:16 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ddadb613fbcb8816395417802a807a74cf45cfaced0bfe66e4dd9147f3872b`  
		Last Modified: Tue, 19 Apr 2022 01:57:22 GMT  
		Size: 4.5 MB (4509399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1750346a0984ac7251aa73e2f2aa2aa50c721d2799d6a51b20eccaa11424c3b6`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309ab00e5b32664715413a02e3a757dae80ef59af68fdbe33b808b5f7697faa7`  
		Last Modified: Tue, 19 Apr 2022 01:57:19 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:ff4d00c43ccc00a0582b1dbc17b5bc28e4ef6545f61b3c6be485e002fae45c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6928061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fc5f4cb0a6e2b6652822c274f5e6bd051757dc7e24c5be03af50467d4ea670`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 05:26:38 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 05:26:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 05:26:42 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 05:26:43 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 05:26:43 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 05:26:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 05:26:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7bcb96bb0f2694c2c3650393794ab8ab1fa8467a8822b1b09ae77d69337c5f`  
		Last Modified: Tue, 19 Apr 2022 05:28:54 GMT  
		Size: 4.5 MB (4502736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526c1a645aeb39ecd91ca84623e21480cad2b868cb28fefc907827db0a6f5ca0`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab0dd3f1cfd48ae336e6ce8fecfd8b004df2828e2e87e0c6ca7c13ef658640`  
		Last Modified: Tue, 19 Apr 2022 05:28:51 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d3813dcd2fc3e0cf5de6843f401b3eafc431455d62833ee7c28c06193a18aa1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7205544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b22a074cac1f81cf6575dd4fd5dee71d17864cff2da4ffca8a61a2fa361ecf2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 03:28:28 GMT
ENV NATS_SERVER=2.8.0
# Tue, 19 Apr 2022 03:28:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6964e92e5d15c1efa29a05f0dd410750c2cf2789097e1391440d7a425108a273' ;; 		armhf) natsArch='arm6'; sha256='4ba6a1fe17fa6d4d65d428ad22afc0cb8aa56ed5486806d179f86ec726c51697' ;; 		armv7) natsArch='arm7'; sha256='3f2d7a38d3d9ea26abda5509177782fc425f79e5d77112093d617904f35663e6' ;; 		x86_64) natsArch='amd64'; sha256='9a6df1121c17dc5537ccb193c2d153b8f3cd1de60a181a41792ea397facce3af' ;; 		x86) natsArch='386'; sha256='d860f618a507124cfb12e5fd0cb42c54513632d004d4d03b3af29c83294d766a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 19 Apr 2022 03:28:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 19 Apr 2022 03:28:33 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 19 Apr 2022 03:28:33 GMT
EXPOSE 4222 6222 8222
# Tue, 19 Apr 2022 03:28:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Apr 2022 03:28:35 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e5206e380b0c366404743459ac59225f405ee55143b5adc2acfce932082a52`  
		Last Modified: Tue, 19 Apr 2022 03:29:38 GMT  
		Size: 4.5 MB (4488093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a12cb300300f405322af040faae4712f2deec744cf03129b35aeb560a07372`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6249060dc7f00f5a65340b45c016b62536f66e152070180fef8946075106d39`  
		Last Modified: Tue, 19 Apr 2022 03:29:37 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
