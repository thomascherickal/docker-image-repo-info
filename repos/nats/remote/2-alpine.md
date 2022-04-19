## `nats:2-alpine`

```console
$ docker pull nats@sha256:84d4a95b9acd9187f768740abfe75abf6bffb5224dcc5cc1a867787f1180354c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

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

### `nats:2-alpine` - linux; arm variant v6

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

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9340cbad2dc025179dc865f5c6f66a69096ded50b2e46afded61ac1f3b412cd9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6866697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f09ecdf2b0aff0fde7ed73027dbc749b7a657349415a11509ae32a4c900514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 15:55:26 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 15:55:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 15:55:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 15:55:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 15:55:31 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 15:55:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:55:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c97ae8e5682d5886f6ccd7ea053da726cc295b9f7293808d4b51ba06210713`  
		Last Modified: Tue, 05 Apr 2022 15:57:37 GMT  
		Size: 4.4 MB (4441372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66714d285cac5fb950706af50a1fbf277ce179d417ca4138c893811e75d820d8`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54375ec28ca00cc6542be4b669aefc6254266ed385d996ce0d2a870b373a4e19`  
		Last Modified: Tue, 05 Apr 2022 15:57:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:939bee059703b05c5b0846c20b51fc00d2400e36f230c70ccbb00f7c5215791c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:067db6f9113d6046cb69c33eae58d0141981d3977f2ae17002944032bff6c30c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:55:12 GMT
ENV NATS_SERVER=2.7.4
# Tue, 05 Apr 2022 08:55:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='49457be98663ef3e128b53b56ba45fca216fb6b0d5ba6841605bd8b3984ab698' ;; 		armhf) natsArch='arm6'; sha256='415e9dbb8fa5de697a3b524d31e15af168758465c17b547f329d14fe158192a2' ;; 		armv7) natsArch='arm7'; sha256='2723c8e7806c552b5c08d5823cbcf36ca7c7657794fae9e6adb9b6b4f1feaea4' ;; 		x86_64) natsArch='amd64'; sha256='1885db0c2844fbfbd07f93e036089f210e8e4b6e4cf0ec3890b3724576afc727' ;; 		x86) natsArch='386'; sha256='16d5a990c0c8ee9ecd275fe1e23cede06c0ae7ca93229738ced1df6b97b8ad6d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Tue, 05 Apr 2022 08:55:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Tue, 05 Apr 2022 08:55:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 05 Apr 2022 08:55:18 GMT
EXPOSE 4222 6222 8222
# Tue, 05 Apr 2022 08:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 08:55:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877eaed0217fc0aefecc8729fcaf3ce7f38ef83f37612dae5c7aebd817496b18`  
		Last Modified: Tue, 05 Apr 2022 08:56:19 GMT  
		Size: 4.4 MB (4426416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a426890e711d28c3849e31785f24b70e6931e1bf1c9aa838bc482ae377e0e7`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ff805262a2c8d64c4660b5f55697e58b27ca330d23f392be3fe262d2f2efd`  
		Last Modified: Tue, 05 Apr 2022 08:56:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
