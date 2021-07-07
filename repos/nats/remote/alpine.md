## `nats:alpine`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:3c2b7ad7052fdc5f13e360dc9b3e3513997b071ec008bd61d3bff3e862c1947a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7434180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49258f52dfceee0babf527ce8158ba3f98a998fa6ff73f8dc05dc67ec2c7a96e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Wed, 07 Jul 2021 00:20:14 GMT
ENV NATS_SERVER=2.3.2
# Wed, 07 Jul 2021 00:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='18a68cbef5c7a41052f5281bdfe9164b51cbeb60ce2dd31a7945c5adbcd39c2d' ;; 		armhf) natsArch='arm6'; sha256='a37949f8a1e24d5a8e47f57786e126205de7c3f6f8b3e5b849f33adbcfe8d2fb' ;; 		armv7) natsArch='arm7'; sha256='43a4820a57161b83fe721b81098d2ba9b1e2f42923be898f031bac40279f8f6e' ;; 		x86_64) natsArch='amd64'; sha256='6e6fdf781465fbf09cb024112b34ae6b2b432d94a5fc8b62f6ebf0da5fc3345d' ;; 		x86) natsArch='386'; sha256='c7c0ea9a5343925f0f5e2dda964946152382b0a3e0db96aa43c3f2ab17a37bf0' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 07 Jul 2021 00:20:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 07 Jul 2021 00:20:18 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 07 Jul 2021 00:20:18 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 00:20:18 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45be4d9f8cb68409d6fb7407ab14ce49d214464c023f641670bfdefab42009a4`  
		Last Modified: Wed, 07 Jul 2021 00:21:10 GMT  
		Size: 4.6 MB (4621729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee574d4f4017f32800275aeefde40b62872bca2876fe91025cdc68dd97f0d8c7`  
		Last Modified: Wed, 07 Jul 2021 00:21:09 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d9cc62817a68bf383b92f18b776f88224028a2c6e33c8df4dcad380c76ec52`  
		Last Modified: Wed, 07 Jul 2021 00:21:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:651fbca389e139956e3f9493a43025cc9ccda1cd955284c17512e5e6e7380644
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6902343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5595c5e3be408f79b509328a9dd4d02282691808e4cf61f0706174c1ba6ee506`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 29 Jun 2021 23:26:34 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 23:26:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4c6bc2eca0ab2e3d1dd2f7d44a2ff82443fbc5ffcd27c8df6506a961b6ced455' ;; 		armhf) natsArch='arm6'; sha256='0c15c293d2e917f9f3450d759663033874ed90143643e18c696eb0cb9e3c9150' ;; 		armv7) natsArch='arm7'; sha256='b9897a69b4448ee00c20251cf7593632770115b4878e1c885c3c4e266a12991c' ;; 		x86_64) natsArch='amd64'; sha256='1478bb7bfacffa5d791edfd98557e68fb236b2b2b7f4c635c99d89e1ab7d8d71' ;; 		x86) natsArch='386'; sha256='f8d4abf66b9a6900dea90f83a5e8d031e1878027c6a69f353a52ea6ea04fc427' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 29 Jun 2021 23:26:39 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 29 Jun 2021 23:26:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 29 Jun 2021 23:26:40 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Jun 2021 23:26:41 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96af6e5ac4162802fb8967e6b4824af5697d8464923ea2c4612d753af2c5a97d`  
		Last Modified: Tue, 29 Jun 2021 23:28:44 GMT  
		Size: 4.3 MB (4276990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258836ae8de6d18aef96b5cbdce103007db494956552d3dddfbc1f7ad0c8b169`  
		Last Modified: Tue, 29 Jun 2021 23:28:41 GMT  
		Size: 559.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce612d2db4df0144be487b883832ee5dea0e09f0d262a6a4bf42495848eff5c`  
		Last Modified: Tue, 29 Jun 2021 23:28:41 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:361ccb5e5d9e37fe2ac39663ac5c9115d6eb0707e106d2da89df73ab69e5715e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6702295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2888e167e3a6de8e686545b2527ac48499dfc9f79ac8d7641c075525df6820fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Wed, 30 Jun 2021 04:57:42 GMT
ENV NATS_SERVER=2.3.1
# Wed, 30 Jun 2021 04:57:47 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4c6bc2eca0ab2e3d1dd2f7d44a2ff82443fbc5ffcd27c8df6506a961b6ced455' ;; 		armhf) natsArch='arm6'; sha256='0c15c293d2e917f9f3450d759663033874ed90143643e18c696eb0cb9e3c9150' ;; 		armv7) natsArch='arm7'; sha256='b9897a69b4448ee00c20251cf7593632770115b4878e1c885c3c4e266a12991c' ;; 		x86_64) natsArch='amd64'; sha256='1478bb7bfacffa5d791edfd98557e68fb236b2b2b7f4c635c99d89e1ab7d8d71' ;; 		x86) natsArch='386'; sha256='f8d4abf66b9a6900dea90f83a5e8d031e1878027c6a69f353a52ea6ea04fc427' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Wed, 30 Jun 2021 04:57:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Wed, 30 Jun 2021 04:57:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Wed, 30 Jun 2021 04:57:49 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:57:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Jun 2021 04:57:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652eb10382c926e7f0177c6edce4e6d87480e4b3ba6084d4c5fc2e46697f0917`  
		Last Modified: Wed, 30 Jun 2021 05:00:01 GMT  
		Size: 4.3 MB (4273408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a9bfea646ffce354fede808fe1ed89e7a1e3096f320bfc8c8eefa37e676d91`  
		Last Modified: Wed, 30 Jun 2021 04:59:59 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1a580a88602526561809683ec350fbdbee085b30d2e8fa6081a4b20bd6cde0`  
		Last Modified: Wed, 30 Jun 2021 04:59:59 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:91786ab43b997798f12cc7f41398cb387bd78db00a1ad22d3593d1cb582759dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6953888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81bff402b580d77b2518d672e5fce6cfd6e5fa744e2e14ad6ad100020ca72607`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Tue, 29 Jun 2021 23:28:47 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 23:28:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4c6bc2eca0ab2e3d1dd2f7d44a2ff82443fbc5ffcd27c8df6506a961b6ced455' ;; 		armhf) natsArch='arm6'; sha256='0c15c293d2e917f9f3450d759663033874ed90143643e18c696eb0cb9e3c9150' ;; 		armv7) natsArch='arm7'; sha256='b9897a69b4448ee00c20251cf7593632770115b4878e1c885c3c4e266a12991c' ;; 		x86_64) natsArch='amd64'; sha256='1478bb7bfacffa5d791edfd98557e68fb236b2b2b7f4c635c99d89e1ab7d8d71' ;; 		x86) natsArch='386'; sha256='f8d4abf66b9a6900dea90f83a5e8d031e1878027c6a69f353a52ea6ea04fc427' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 29 Jun 2021 23:28:51 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 29 Jun 2021 23:28:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 29 Jun 2021 23:28:51 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:28:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Jun 2021 23:28:52 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a20cc896bef35ff639511c8e76c91d5908bfcf095dcebc4d32c42a3679b1fca`  
		Last Modified: Tue, 29 Jun 2021 23:30:09 GMT  
		Size: 4.2 MB (4243290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d6b1224ace504c1cb829e06b31639587fe97cf8f83a651d1c6c6002cc6f000`  
		Last Modified: Tue, 29 Jun 2021 23:30:08 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6306ef7db7ec419a5f78104db2200f17a99ddf9ed8e963001faeaca00410dab8`  
		Last Modified: Tue, 29 Jun 2021 23:30:08 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
