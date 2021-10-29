## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:a4a52bf9a4848b0019a2e95d30237f6cc54d6a5ed71f4a1b4114c6a92cea1f98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:adc1833a9cd2c661dbcccde26963c38933760e2305b56cf947e35d713cd888f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7665355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d9f197f2ae1ebaccf4547005f1251db5919826f92c27b2c712d613201d683a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:19:43 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:19:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:19:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:19:47 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:19:48 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48177a83f998a02030b8eeff8c4ec7d357cfadd8d9a3c83edc17fc7d69f1b603`  
		Last Modified: Thu, 28 Oct 2021 22:20:26 GMT  
		Size: 4.8 MB (4849934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84343717d682bb0de25deea9ce71d48383ceb7bb816345a4d7821c9906fcf1b`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b90f3e5ed62b20adc570a3fca67fef39d1639334380a7a02d1ec648f806fc`  
		Last Modified: Thu, 28 Oct 2021 22:20:25 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:f18f0559e6592f476ed3c324119e679bae76a3412575087afb9ce6e2873d80eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f29a7de02223b95daa0fea80405b6b7c6609a4690dcc2917d9aa8eaffe5ac0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 23:05:46 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 23:05:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 23:05:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 23:05:52 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 23:05:52 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:05:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 23:05:53 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09b4d6b98e1fd4df5c98b8b5158ce503a9a27a62d966c9b38b3f741d8cab81`  
		Last Modified: Thu, 28 Oct 2021 23:07:59 GMT  
		Size: 4.5 MB (4512878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d9bebc37ed822cf9acbab6cff1de83d7abe6e413e8af544a664a35ebfae0dc`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc2246851158b6d3e62406a9838af451bde9cae7c355f8d23712f226dc987fd`  
		Last Modified: Thu, 28 Oct 2021 23:07:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:241204375d0421fafa36f007a727187dc13b6699a006788dbe9f9053db06776b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6939749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abf44c1a9986a622b3ab649cdae404a16fbf3103c0caa07b274da2294988b2fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 29 Oct 2021 01:08:39 GMT
ENV NATS_SERVER=2.6.3
# Fri, 29 Oct 2021 01:08:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 29 Oct 2021 01:08:44 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 29 Oct 2021 01:08:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Oct 2021 01:08:45 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Oct 2021 01:08:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebe08fb6402137fadd25be1fc438da637104869e2ab8849246cc5a5f9f2f2a6`  
		Last Modified: Fri, 29 Oct 2021 01:10:59 GMT  
		Size: 4.5 MB (4508359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ead296b2f42ccf22cfbbf50012871189a98a180bb39f3e40a9149048f87ab`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 557.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9391a1774ef75f6a6eb537a456e01e2af021a66ad8e2474bc06286d2dc6e3607`  
		Last Modified: Fri, 29 Oct 2021 01:10:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91519e4dc20857e393ceb60cfd6c775e9ca1df577eb15f33098b24bc665085bd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7174773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50e83d48e20732e08a03a5c028e7099a1cb22486ce2ff0ca3d421105f6ab4e72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 28 Oct 2021 22:43:36 GMT
ENV NATS_SERVER=2.6.3
# Thu, 28 Oct 2021 22:43:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='ee7f3782fa6b3be4a3be33bb144279993ac2624d2f26cfae1e53001ac56d3fc0' ;; 		armhf) natsArch='arm6'; sha256='0adf63fc6c4084f53cbc50a6eedc43e6cec77e6d497eb79d7e429aa49189b40f' ;; 		armv7) natsArch='arm7'; sha256='f36135c54a1409a4212a84fa40dfbc46049abd8f6e00c7da35d02bdbd5e63584' ;; 		x86_64) natsArch='amd64'; sha256='91232ce15ae9ac408fea4ab1553bbc21a32f79d580e2ff28352c1de30bc8e089' ;; 		x86) natsArch='386'; sha256='a4342321405eb62819ef287d4b2d48d3d628a611130960aa4ed3fb58b821d34d' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Thu, 28 Oct 2021 22:43:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Thu, 28 Oct 2021 22:43:42 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Oct 2021 22:43:42 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Oct 2021 22:43:44 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a9bddb5b6dea1e03bbcefb3ec30c51fdeb2aaed372a5a18267b809289d14a7`  
		Last Modified: Thu, 28 Oct 2021 22:44:41 GMT  
		Size: 4.5 MB (4462004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826bc0279c52e103635837d546f00f6db710f97485f10b238b6af7062999563d`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668fe846a6f8a9180a2f7b42b425ae86673882581ab869770d6ce79d3049a5c6`  
		Last Modified: Thu, 28 Oct 2021 22:44:40 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
