<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.14`](#nats2-alpine314)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2-windowsservercore-ltsc2016`](#nats2-windowsservercore-ltsc2016)
-	[`nats:2.3`](#nats23)
-	[`nats:2.3-alpine`](#nats23-alpine)
-	[`nats:2.3-alpine3.14`](#nats23-alpine314)
-	[`nats:2.3-linux`](#nats23-linux)
-	[`nats:2.3-nanoserver`](#nats23-nanoserver)
-	[`nats:2.3-nanoserver-1809`](#nats23-nanoserver-1809)
-	[`nats:2.3-scratch`](#nats23-scratch)
-	[`nats:2.3-windowsservercore`](#nats23-windowsservercore)
-	[`nats:2.3-windowsservercore-1809`](#nats23-windowsservercore-1809)
-	[`nats:2.3-windowsservercore-ltsc2016`](#nats23-windowsservercore-ltsc2016)
-	[`nats:2.3.1`](#nats231)
-	[`nats:2.3.1-alpine`](#nats231-alpine)
-	[`nats:2.3.1-alpine3.14`](#nats231-alpine314)
-	[`nats:2.3.1-linux`](#nats231-linux)
-	[`nats:2.3.1-nanoserver`](#nats231-nanoserver)
-	[`nats:2.3.1-nanoserver-1809`](#nats231-nanoserver-1809)
-	[`nats:2.3.1-scratch`](#nats231-scratch)
-	[`nats:2.3.1-windowsservercore`](#nats231-windowsservercore)
-	[`nats:2.3.1-windowsservercore-1809`](#nats231-windowsservercore-1809)
-	[`nats:2.3.1-windowsservercore-ltsc2016`](#nats231-windowsservercore-ltsc2016)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.14`](#natsalpine314)
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
$ docker pull nats@sha256:3ebddc416bf564c582a74b9e3586a3156c2cb12538ca779c762ffb67dd03298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

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

### `nats:2-alpine` - linux; arm variant v6

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

### `nats:2-alpine` - linux; arm variant v7

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

### `nats:2-alpine` - linux; arm64 variant v8

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

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

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

### `nats:2-alpine3.14` - linux; arm variant v6

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

### `nats:2-alpine3.14` - linux; arm variant v7

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

### `nats:2-alpine3.14` - linux; arm64 variant v8

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

## `nats:2-linux`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:99d4d10f24f941d79ccfae266b8a46442230cce0a9b704e52616ca92965f463c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:93ac3cd4a8b8b007880643270736917965c1417da426af8f293014475ac55768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:5f2213e66ca2e80cb5c9702bbec42f68edf0a8a997510126714a42e544d0e51e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3`

```console
$ docker pull nats@sha256:3ebddc416bf564c582a74b9e3586a3156c2cb12538ca779c762ffb67dd03298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-alpine`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine` - linux; amd64

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

### `nats:2.3-alpine` - linux; arm variant v6

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

### `nats:2.3-alpine` - linux; arm variant v7

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

### `nats:2.3-alpine` - linux; arm64 variant v8

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

## `nats:2.3-alpine3.14`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-alpine3.14` - linux; amd64

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

### `nats:2.3-alpine3.14` - linux; arm variant v6

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

### `nats:2.3-alpine3.14` - linux; arm variant v7

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

### `nats:2.3-alpine3.14` - linux; arm64 variant v8

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

## `nats:2.3-linux`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-nanoserver-1809`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-scratch`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore`

```console
$ docker pull nats@sha256:99d4d10f24f941d79ccfae266b8a46442230cce0a9b704e52616ca92965f463c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2.3-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:93ac3cd4a8b8b007880643270736917965c1417da426af8f293014475ac55768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:5f2213e66ca2e80cb5c9702bbec42f68edf0a8a997510126714a42e544d0e51e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1`

```console
$ docker pull nats@sha256:e976c394120e489ed76b54ef3a4cc2ff9bbe34161aaa623070216204131ce123
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3.1` - linux; amd64

```console
$ docker pull nats@sha256:6c306d5b71b2ec5a796708b88b4ae8e344650a7ab045b8936c9355cda478cdd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4337895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec646edfb434bc83799a0c385e1158b1402ee3582ce7ec43793ffd8f78ce0e1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:c7f8cc94da3e7d82f3e7fc2102bfdc68ebf26a85ec387d7c7f9557ec3ad21013 in /nats-server 
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 22:38:09 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:38:09 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 22:38:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d701534f1611c69546f8dc7b72d71cb1c8f0e3502bc99ebba9e6eb256639a982`  
		Last Modified: Tue, 29 Jun 2021 22:39:06 GMT  
		Size: 4.3 MB (4337419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1784a8fbf4379872a33242fa1271f3758fd54ad6c6b83158f801b42532c7a1`  
		Last Modified: Tue, 29 Jun 2021 22:39:05 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-alpine`

```console
$ docker pull nats@sha256:8e3fd5de8c5ec5bd9055ae6a38acad7e7c42aba840e09f603c667e9f2f069b43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.1-alpine` - linux; amd64

```console
$ docker pull nats@sha256:01ac0855814ed7de4babe3b6651f5c3da3f33eaf038822ded00ed00e54192116
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7432880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59ffd974b2230b5c75b03bb1436e0d3552d35b7ffb4444dc27920fedc46826a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 29 Jun 2021 22:37:22 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:37:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4c6bc2eca0ab2e3d1dd2f7d44a2ff82443fbc5ffcd27c8df6506a961b6ced455' ;; 		armhf) natsArch='arm6'; sha256='0c15c293d2e917f9f3450d759663033874ed90143643e18c696eb0cb9e3c9150' ;; 		armv7) natsArch='arm7'; sha256='b9897a69b4448ee00c20251cf7593632770115b4878e1c885c3c4e266a12991c' ;; 		x86_64) natsArch='amd64'; sha256='1478bb7bfacffa5d791edfd98557e68fb236b2b2b7f4c635c99d89e1ab7d8d71' ;; 		x86) natsArch='386'; sha256='f8d4abf66b9a6900dea90f83a5e8d031e1878027c6a69f353a52ea6ea04fc427' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 29 Jun 2021 22:37:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 29 Jun 2021 22:37:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 29 Jun 2021 22:37:26 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Jun 2021 22:37:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d831c05385bef516e1aa18acbd6c5a6e5342f1ee94c9ff956653d3ae78dc15`  
		Last Modified: Tue, 29 Jun 2021 22:38:38 GMT  
		Size: 4.6 MB (4620434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e806020ca1351bc64767b4c4f3cae748c55cc220310e336e2fed9a733d7742`  
		Last Modified: Tue, 29 Jun 2021 22:38:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1464f5700c2c8178c092da4b6d5f28bfb0d21bf45cabf7475ed92f9cf61d1e6`  
		Last Modified: Tue, 29 Jun 2021 22:38:36 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-alpine` - linux; arm variant v6

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

### `nats:2.3.1-alpine` - linux; arm variant v7

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

### `nats:2.3.1-alpine` - linux; arm64 variant v8

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

## `nats:2.3.1-alpine3.14`

```console
$ docker pull nats@sha256:8e3fd5de8c5ec5bd9055ae6a38acad7e7c42aba840e09f603c667e9f2f069b43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.1-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:01ac0855814ed7de4babe3b6651f5c3da3f33eaf038822ded00ed00e54192116
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7432880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59ffd974b2230b5c75b03bb1436e0d3552d35b7ffb4444dc27920fedc46826a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 29 Jun 2021 22:37:22 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:37:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='4c6bc2eca0ab2e3d1dd2f7d44a2ff82443fbc5ffcd27c8df6506a961b6ced455' ;; 		armhf) natsArch='arm6'; sha256='0c15c293d2e917f9f3450d759663033874ed90143643e18c696eb0cb9e3c9150' ;; 		armv7) natsArch='arm7'; sha256='b9897a69b4448ee00c20251cf7593632770115b4878e1c885c3c4e266a12991c' ;; 		x86_64) natsArch='amd64'; sha256='1478bb7bfacffa5d791edfd98557e68fb236b2b2b7f4c635c99d89e1ab7d8d71' ;; 		x86) natsArch='386'; sha256='f8d4abf66b9a6900dea90f83a5e8d031e1878027c6a69f353a52ea6ea04fc427' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Tue, 29 Jun 2021 22:37:25 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Tue, 29 Jun 2021 22:37:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Tue, 29 Jun 2021 22:37:26 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:37:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Jun 2021 22:37:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d831c05385bef516e1aa18acbd6c5a6e5342f1ee94c9ff956653d3ae78dc15`  
		Last Modified: Tue, 29 Jun 2021 22:38:38 GMT  
		Size: 4.6 MB (4620434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e806020ca1351bc64767b4c4f3cae748c55cc220310e336e2fed9a733d7742`  
		Last Modified: Tue, 29 Jun 2021 22:38:36 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1464f5700c2c8178c092da4b6d5f28bfb0d21bf45cabf7475ed92f9cf61d1e6`  
		Last Modified: Tue, 29 Jun 2021 22:38:36 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-alpine3.14` - linux; arm variant v6

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

### `nats:2.3.1-alpine3.14` - linux; arm variant v7

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

### `nats:2.3.1-alpine3.14` - linux; arm64 variant v8

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

## `nats:2.3.1-linux`

```console
$ docker pull nats@sha256:2c1fb2a7cb40a9d9315b3946c80b36335460c98595fce092acd7ceac2954a732
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.1-linux` - linux; amd64

```console
$ docker pull nats@sha256:6c306d5b71b2ec5a796708b88b4ae8e344650a7ab045b8936c9355cda478cdd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4337895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec646edfb434bc83799a0c385e1158b1402ee3582ce7ec43793ffd8f78ce0e1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:c7f8cc94da3e7d82f3e7fc2102bfdc68ebf26a85ec387d7c7f9557ec3ad21013 in /nats-server 
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 22:38:09 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:38:09 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 22:38:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d701534f1611c69546f8dc7b72d71cb1c8f0e3502bc99ebba9e6eb256639a982`  
		Last Modified: Tue, 29 Jun 2021 22:39:06 GMT  
		Size: 4.3 MB (4337419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1784a8fbf4379872a33242fa1271f3758fd54ad6c6b83158f801b42532c7a1`  
		Last Modified: Tue, 29 Jun 2021 22:39:05 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-nanoserver`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3.1-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-nanoserver-1809`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3.1-nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-scratch`

```console
$ docker pull nats@sha256:2c1fb2a7cb40a9d9315b3946c80b36335460c98595fce092acd7ceac2954a732
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.3.1-scratch` - linux; amd64

```console
$ docker pull nats@sha256:6c306d5b71b2ec5a796708b88b4ae8e344650a7ab045b8936c9355cda478cdd2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4337895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec646edfb434bc83799a0c385e1158b1402ee3582ce7ec43793ffd8f78ce0e1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:c7f8cc94da3e7d82f3e7fc2102bfdc68ebf26a85ec387d7c7f9557ec3ad21013 in /nats-server 
# Tue, 29 Jun 2021 22:38:08 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 22:38:09 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:38:09 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 22:38:09 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d701534f1611c69546f8dc7b72d71cb1c8f0e3502bc99ebba9e6eb256639a982`  
		Last Modified: Tue, 29 Jun 2021 22:39:06 GMT  
		Size: 4.3 MB (4337419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1784a8fbf4379872a33242fa1271f3758fd54ad6c6b83158f801b42532c7a1`  
		Last Modified: Tue, 29 Jun 2021 22:39:05 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-windowsservercore`

```console
$ docker pull nats@sha256:99d4d10f24f941d79ccfae266b8a46442230cce0a9b704e52616ca92965f463c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:2.3.1-windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.3.1-windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-windowsservercore-1809`

```console
$ docker pull nats@sha256:93ac3cd4a8b8b007880643270736917965c1417da426af8f293014475ac55768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:2.3.1-windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.3.1-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:5f2213e66ca2e80cb5c9702bbec42f68edf0a8a997510126714a42e544d0e51e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:2.3.1-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:595e851d5a9f339d70f0e96de05759579a484f643584f0a6534f98ee0fad9c02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

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

### `nats:alpine3.14` - linux; arm variant v6

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

### `nats:alpine3.14` - linux; arm variant v7

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

### `nats:alpine3.14` - linux; arm64 variant v8

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

## `nats:latest`

```console
$ docker pull nats@sha256:3ebddc416bf564c582a74b9e3586a3156c2cb12538ca779c762ffb67dd03298a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1999; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:a702a304917f94f6f26c89b1be863043201737b87c03ae87966cb045d1adeabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:c473e6c9bdf5caa94b125d428e0c776cfb0e74ddecd6b36e2a861ad0fa767eae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107075200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00bc8be898b16d90245ca1f63556beb9e3a0edb7a043553b938a990923a026ed`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 15:55:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:06 GMT
RUN cmd /S /C #(nop) COPY file:c3edaafca1bac336e219c6dd6ca6992a1a25a0d6e709941f7269ff18fe8f62e8 in C:\nats-server.exe 
# Tue, 29 Jun 2021 22:18:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:18:12 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:18:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:18:18 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:80d93ce19113bbf944b699f12e59395e0eabeb00ccd1fd5dc7df46bb115eba2f`  
		Last Modified: Wed, 09 Jun 2021 15:59:58 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd03a2da7740641352b48102d34749bc6f85bc0ccca5fa16975176229824514`  
		Last Modified: Tue, 29 Jun 2021 22:22:41 GMT  
		Size: 4.4 MB (4397348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2acb4c1ba564809b4b555f9ab92527cd82acca70412b814616b2cba4ec5680`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a1fee7bf5bdcfcda84d5b05f8f5808c8d1c6773b1a3fd09adce0417dcd33e9`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416251dadd3dad79c0945337f22c8c4686d8229929c5fe7a4e9f22c0ab11f51e`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac4c5bd3ec0b0519cd82d25bc85011b0035679f1cb250262ea2500c76ed477a`  
		Last Modified: Tue, 29 Jun 2021 22:22:40 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:99d4d10f24f941d79ccfae266b8a46442230cce0a9b704e52616ca92965f463c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `nats:windowsservercore` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:93ac3cd4a8b8b007880643270736917965c1417da426af8f293014475ac55768
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.1999; amd64

```console
$ docker pull nats@sha256:dfc1674cec617d038182099763e8e21ae02caab5b0cbcdf3b294b164cfba144d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646702292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891b94f87075103849e518eb50b76433a17ada32f8d1cf5aa36e530521d6a7ab`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:52:54 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:16:09 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:16:11 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:16:14 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:16:42 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:17:43 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:17:46 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:17:48 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:17:50 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:17:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507a90d55d261855b42c7b5905599cdc274ca135ad962fffffe1fa6246c9bba7`  
		Last Modified: Wed, 09 Jun 2021 15:59:38 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c372ca63b1680d65d6a15156585166129bcfbe52e0d05d0054fb79aef686c21`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d56dca1f1579b9ec59f1d6041c16b91b6f68baf0084499e2a85c1405d969db`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e1b684efe630f2971519c8b17b93b91570783e8fbdf7e7ec7f29b55debfca4`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99faa4fc39833933dd9eb1cbf6b84eccc63727e8b32eb4705e1dec20166b5a49`  
		Last Modified: Tue, 29 Jun 2021 22:22:22 GMT  
		Size: 363.9 KB (363912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ee24bc113845fef06be0fc93dcd98e34aa2e27e9623df01a966b142e697c5f`  
		Last Modified: Tue, 29 Jun 2021 22:22:25 GMT  
		Size: 4.7 MB (4740124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e272136ec5116ad206285b67f3beb3298d68d6c96273dae139b98b326d71cef`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 2.0 KB (1958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b975b0b42baf2261e7a3ebb135c8b398592c2445b335b404cee3476917b4ab4a`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a43a208d117f790575104759c3ad082ad2d1e74663fe794882536de5c7934d1`  
		Last Modified: Tue, 29 Jun 2021 22:22:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c7916c3fd7bebe37b25576dd2b9f6d9b72be1b48773da796349d7ef3058365`  
		Last Modified: Tue, 29 Jun 2021 22:22:20 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:5f2213e66ca2e80cb5c9702bbec42f68edf0a8a997510126714a42e544d0e51e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull nats@sha256:c7d974ffec99dcd05b0e18a657825d3a8bcdf8f805b52b83ea1cf19835748efb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6275287446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4052c7a4a55e8293e15160c8c2b452d7a87489af0e64522d5b32ad744db41f59`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 15:55:27 GMT
ENV NATS_DOCKERIZED=1
# Tue, 29 Jun 2021 22:18:26 GMT
ENV NATS_SERVER=2.3.1
# Tue, 29 Jun 2021 22:18:29 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.3.1/nats-server-v2.3.1-windows-amd64.zip
# Tue, 29 Jun 2021 22:18:31 GMT
ENV NATS_SERVER_SHASUM=aad71bfbbd71f355b80bd202358a682413e3c0a1884b43049182184f86b29943
# Tue, 29 Jun 2021 22:19:31 GMT
RUN Set-PSDebug -Trace 2
# Tue, 29 Jun 2021 22:21:26 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Tue, 29 Jun 2021 22:21:28 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Tue, 29 Jun 2021 22:21:30 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 22:21:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 29 Jun 2021 22:21:35 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db57f94547be7109ad927e2f9d04a0501a2a5f0cb91ad8c4385eb32758f86b9`  
		Last Modified: Wed, 09 Jun 2021 16:00:21 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c2d7bc13e759389bf1965f0d8677dd643b0408a429a502d70c2b1bf1cc3a15`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194a1a3dbb25a5be33d59b6fa621a1bf62a7e60b1135389c20439e87555a83e`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7981429ef0cc31c2c8554645f34b3c993bd795f7a7d7b360d20b5dfe1f2794a0`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8215cc8e154ef4991f9596c105dd937301dc23e4cb2f612b841c636b7b4db`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 323.7 KB (323681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d7dd0d695458c4dd8adaf26ee4da1d63e8fcb8a3b3e405f9f48264fba159ea`  
		Last Modified: Tue, 29 Jun 2021 22:23:00 GMT  
		Size: 9.2 MB (9223377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557dd623519022f791f727cc39a7d74c08358ea9f5ea3c1e91b9632ce735056`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 2.0 KB (1976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415226cfd0e0b87dab1e79fc91300544dd70a0cacb4124fd481d9ea4fad93901`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855a140e928acc9bfc880f6c20f92834784a99dc16cf18571e3c7bce5d1966e8`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a2c24376be4fa44460f475c858c8714b958a5a13eae47e6f64231c25636f92`  
		Last Modified: Tue, 29 Jun 2021 22:22:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
