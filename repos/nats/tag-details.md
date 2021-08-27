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
-	[`nats:2.4`](#nats24)
-	[`nats:2.4-alpine`](#nats24-alpine)
-	[`nats:2.4-alpine3.14`](#nats24-alpine314)
-	[`nats:2.4-linux`](#nats24-linux)
-	[`nats:2.4-nanoserver`](#nats24-nanoserver)
-	[`nats:2.4-nanoserver-1809`](#nats24-nanoserver-1809)
-	[`nats:2.4-scratch`](#nats24-scratch)
-	[`nats:2.4-windowsservercore`](#nats24-windowsservercore)
-	[`nats:2.4-windowsservercore-1809`](#nats24-windowsservercore-1809)
-	[`nats:2.4-windowsservercore-ltsc2016`](#nats24-windowsservercore-ltsc2016)
-	[`nats:2.4.0`](#nats240)
-	[`nats:2.4.0-alpine`](#nats240-alpine)
-	[`nats:2.4.0-alpine3.14`](#nats240-alpine314)
-	[`nats:2.4.0-linux`](#nats240-linux)
-	[`nats:2.4.0-nanoserver`](#nats240-nanoserver)
-	[`nats:2.4.0-nanoserver-1809`](#nats240-nanoserver-1809)
-	[`nats:2.4.0-scratch`](#nats240-scratch)
-	[`nats:2.4.0-windowsservercore`](#nats240-windowsservercore)
-	[`nats:2.4.0-windowsservercore-1809`](#nats240-windowsservercore-1809)
-	[`nats:2.4.0-windowsservercore-ltsc2016`](#nats240-windowsservercore-ltsc2016)
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
$ docker pull nats@sha256:45ba1e75b73aa90e7005aa09c5991b299bf4a5523d5ceaa0644005aea14bd0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.14`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4`

```console
$ docker pull nats@sha256:45ba1e75b73aa90e7005aa09c5991b299bf4a5523d5ceaa0644005aea14bd0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-alpine`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-alpine3.14`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-linux`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4-linux` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-scratch`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4-scratch` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0`

```console
$ docker pull nats@sha256:45ba1e75b73aa90e7005aa09c5991b299bf4a5523d5ceaa0644005aea14bd0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-alpine`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4.0-alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-alpine3.14`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4.0-alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-linux`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4.0-linux` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-scratch`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.4.0-scratch` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4.0-windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.4.0-windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:2.4.0-windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.4.0-windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:2.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.14`

```console
$ docker pull nats@sha256:46e53166a270226c1940d495bf2d2fc5d8adb4f150ab62822bc6334af9795b96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.14` - linux; amd64

```console
$ docker pull nats@sha256:79f20bf7572a9763a44766834077189f1c775889653cd06074cd253411e57a61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7630738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1cf25eec293c91bbdbf8b721d5bf624068f661f44e98e1e205e8c229cab087`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:44:58 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:45:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:45:01 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:45:01 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:45:02 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959ebfdebb025023622bfeb78dc3a9beb3090fa18b8697942c7dc6f0b87afa99`  
		Last Modified: Fri, 27 Aug 2021 20:45:51 GMT  
		Size: 4.8 MB (4815326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f228a428ebd569f8107874e30b71d5b203f766eba63c7978d3c235ba9b2c275f`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe1003110185dc217624a0a61a29d552bff59dd5db5fb81644dfe9638e12c14a`  
		Last Modified: Fri, 27 Aug 2021 20:45:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v6

```console
$ docker pull nats@sha256:d2970c337c556520a6a401a42359b55640f2f281d2635c60766dc0520e25b57e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7110997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53a21416e0b5450b0419dfbc19c701988335fb81af41400f9d53a6ace87d9689`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:21:13 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 19:21:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 19:21:19 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 19:21:20 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 19:21:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 19:21:20 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b6e09a2b90a93499c1ceb83dc1c69831a23a4bc750ed302270c396310e6f`  
		Last Modified: Fri, 27 Aug 2021 19:23:20 GMT  
		Size: 4.5 MB (4482583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77add155971e16911d39c7665575fca22ae70e7678c2eb2273f8c0e2917cd650`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443a5dedeb43279bb9f645efa3abb4ad50e3bcb33a70993793a7018568d3b4`  
		Last Modified: Fri, 27 Aug 2021 19:23:18 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm variant v7

```console
$ docker pull nats@sha256:9fdddb77b45992dd28913e9dfa6bc38fbec5529bd6e2ebfee5a3062adb65d3db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6909360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6f14d25a2d94b56f2a9f861be0b92583a98fa9ea527df32150655256018ff97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:12:43 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 21:12:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 21:12:48 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 21:12:49 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 21:12:49 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 21:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 21:12:50 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5966a7cedc8cd3fd86581316ea0c056ee1beab3cece3b6cc4dd672fc46540baf`  
		Last Modified: Fri, 27 Aug 2021 21:14:56 GMT  
		Size: 4.5 MB (4477972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad6a30f2c8e55902fd5341442838c84cedf23c949539cdfd87d76f6176d5dda`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 558.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6c2ea642bdc0a92a6797a6e2ea5891f8e13439fd7eeba41e56b6ffda56bb68`  
		Last Modified: Fri, 27 Aug 2021 21:14:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.14` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:54296f6b2e2f9ad2f2d915cb051bb5488c1886e10fb3113dab8beccfea099f3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367117c3b6999bbce81500a1b91d45c285421492dba487dc26e6a77b0ae3b15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:13:00 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 20:13:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='eb510dd016cb1a9e9b1fae88a3471029048cb75dcc4ad83a4f5b1e3665f24a20' ;; 		armhf) natsArch='arm6'; sha256='76ac66cd86217a43bc227220eb054aac8a5744890d43c76156075d68a684d9e0' ;; 		armv7) natsArch='arm7'; sha256='e7521841d59f55fcef6172aa8f22d3af7ba1776bd67109a23c29d34d18d44bd6' ;; 		x86_64) natsArch='amd64'; sha256='f6841c89fcf99302bc7ac295ddc1e75322385f861d55abee79733976c8eb9bc7' ;; 		x86) natsArch='386'; sha256='c7e6e2b73d402e841b3abb57e26e2ef53350b44e385255bf289b08182058076a' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 	apk add --no-cache --virtual buildtmp; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}"; 		apk del --no-cache --no-network buildtmp
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /etc/nats/nats-server.conf 
# Fri, 27 Aug 2021 20:13:03 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 27 Aug 2021 20:13:03 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 20:13:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 Aug 2021 20:13:04 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788ae5a961ca39ee2b8ce63e18be57be837da6709872417f61ff58acfadac9`  
		Last Modified: Fri, 27 Aug 2021 20:14:08 GMT  
		Size: 4.4 MB (4432320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370dbc05c61e458a187a96a04e44ec07f0255fbd890b0a83bbca97e35a608b0`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2363b7bda10d7281126914d156597af49cf232101dd830d492c404d69e008`  
		Last Modified: Fri, 27 Aug 2021 20:14:07 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:45ba1e75b73aa90e7005aa09c5991b299bf4a5523d5ceaa0644005aea14bd0a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:21ff4cbb5485b408bcc030f341817018fb13a7381ca7c520960bf26bab74ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:9c370308b1924738df19dd502a9d8d8c13066580fd1550eddbf4f70663c87fe5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107338949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90920ed24cf8337e7f99fdd7199bff8ec7dd43cfa5063f0f373e6700f8a17a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:bafd3fc1559b39648f01fab1b3b19a9fc9bb95afae5b07b1d7987b376806e053 in C:\nats-server.exe 
# Fri, 27 Aug 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb815244c76bae445a6697a3f1b6a0643fc016be2b2da5192dc6bb4079cd0119`  
		Last Modified: Fri, 27 Aug 2021 00:20:21 GMT  
		Size: 4.6 MB (4591622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33193ffa3c81a2ebd95cb6af96ce80ee557191a64ba47e1977479e1167530ca`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c57e2e68d87e03a37f706b01fe403fc34435b82da71d1080e11ec9df4d418a2`  
		Last Modified: Fri, 27 Aug 2021 00:20:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048b1707f600e77fb06d48bd9c3759cad471944658bdfa3dd59b2852dc7983b4`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b434e68e7546ed285144b98ef8fc3a10f1b6ee578ef2503e9f09aefab0370d0`  
		Last Modified: Fri, 27 Aug 2021 00:20:20 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:0e3da4bd4949f156933e44268ff3e81307b1715fe8a8f4c78885f08a11806326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:35ff92bfc7e822eab96fe3d712164f6b547c3acffc8691b80528d334283849ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4535346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:165538b9f99adf71764e6e01627236bc7de03587ef8c39b621c159491466465e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:c88c76fcaa944eb4751e2b3c987b59dd654a42db7426be2223f22a0698cd6e5c in /nats-server 
# Fri, 27 Aug 2021 03:35:09 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:35:09 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:35:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:35:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d96e79a5881296813985815a1fa73e2441e72769541b1fb32a0e14f2acf4d659`  
		Last Modified: Fri, 27 Aug 2021 03:36:00 GMT  
		Size: 4.5 MB (4534870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04479ea8ab2597ba1679773da48df06a9e646e3e7b67b0eb2c8c0bc6c51eb598`  
		Last Modified: Fri, 27 Aug 2021 03:35:59 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:7201c8cd794776fa392c3a25eb89e4ee987aeaaae647caa364621d5daf5ca3c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4201703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2211a135c8d5c9641c74ba5d54c3c1df4ac3f24fa70a6a57be8a2975af7854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:81d7dcb1f2223ae767ee02f3b24758797ca55a665d17dcb2054eeb097fb2eafa in /nats-server 
# Fri, 27 Aug 2021 02:48:56 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 02:48:57 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 02:48:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 02:48:58 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a820d11a96d84195887c44533ffcad67997fcb79d52f4564709bfdbde47d578d`  
		Last Modified: Fri, 27 Aug 2021 02:51:18 GMT  
		Size: 4.2 MB (4201229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1c4f82bf849dc3d9d18f1c560b9afd0e5237eb2f05377e6792dda2480249cb`  
		Last Modified: Fri, 27 Aug 2021 02:51:15 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:f2057644b631cd588b9ef8800c17a98848297ef9e8b14e896c6637c419716372
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4196286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4e34b9a7771c2092b58b5d6f99401eee0374e56201d34a1c7f84d6f53c05428`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 04:12:30 GMT
COPY file:6576d0950936fbd8cd0ba8e9a7c8094950f25bd1a90d55b60e3e65ea2042854c in /nats-server 
# Fri, 27 Aug 2021 04:12:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 04:12:31 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 04:12:32 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 04:12:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d135e76e7d6d665dbc290a175c8ae8ecfb2ca0aa9f3a2ba24b7dccf731e64cde`  
		Last Modified: Fri, 27 Aug 2021 04:14:54 GMT  
		Size: 4.2 MB (4195812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc14281759482e956b9f087159fb1610c9a80c3fe13daec5850693cafea3d3d`  
		Last Modified: Fri, 27 Aug 2021 04:14:51 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:f5540c14ed29a1ef1c754918bc89f829f49fd6580803a9219f5d1cd554338b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4148379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56533e4f95e8c4154db8d7717a0b0435a0ce0888125cfd0e4087543db765a6bc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:61407b2494616881c09d27c01bdb5a1169dbf9163831a2352284c5578e6cdaad in /nats-server 
# Fri, 27 Aug 2021 03:19:15 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 27 Aug 2021 03:19:16 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 03:19:16 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 Aug 2021 03:19:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3c5d1fa5c137082797b53a6d9ed69aceb52e853695ee3bf824776ad6f0d2b753`  
		Last Modified: Fri, 27 Aug 2021 03:20:37 GMT  
		Size: 4.1 MB (4147902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbae3f13cb6757dadd56bd833076486ed81b2c1c87b7b3ca721e459d8f477b6`  
		Last Modified: Fri, 27 Aug 2021 03:20:36 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:cf3aae4f841ee35ce5bfef42265fbd8025c1cff06d3f284e813cfec4cf9d6e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2114; amd64
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:windowsservercore` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:a328e744c3a06f930890900c486761a97c2108563a63a093b1d0fc0fb9a1ad21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:48cc63b49c047b98135531fccf1f7c4a418477d38def8702f6ecce6e8574923c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2691328041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3d57b266e04d58ceedd30a6c5428caa6783ca301ecc858c8aa62a8f682a3a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 25 Aug 2021 13:46:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:05:30 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:14:05 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:14:06 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:14:07 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:15:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:16:22 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:16:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:16:24 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:16:25 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:16:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:985da5cbc0735e1c422e766af23125ba345f431cb337ea43ec32298d0bb8e4ea`  
		Last Modified: Wed, 25 Aug 2021 15:45:02 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dbdd68a4b0c278695b3e1d401d7eddfb0f0e3aa1e28aed88eb700059648f8f`  
		Last Modified: Wed, 25 Aug 2021 16:11:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9924833e15cbbaa8bd2d64c942c877c0765ba95d0790a5a9ea83a3d40bcaba43`  
		Last Modified: Fri, 27 Aug 2021 00:20:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b8b51ab5e087ce5a5187d2967b0a82e4ce38b2151fc1b040be11a843334b1a`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73666a2686d6829048f4fa9f037f08038370c72202369f80bd4b715ead2cafe3`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35fdb95a7dc56c84ff744d8172574e2edd053f77affad83306be03c14fdb9fb`  
		Last Modified: Fri, 27 Aug 2021 00:20:01 GMT  
		Size: 372.5 KB (372513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b9b9590a746c11677c6728f047f437a87645f68249b9691ed347591b850b8d`  
		Last Modified: Fri, 27 Aug 2021 00:20:00 GMT  
		Size: 4.9 MB (4944435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b629e22fb2c409b07df4f55a5b1c1d392ae3fc7110b646f46f63c8de8af0f470`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 2.0 KB (1978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c15056241134a8112b0c3e43493f7be7cd0421808ee5edbddb6490f355110e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b1ee4ad1c87cc30317f9c2212c416f2a120923e62f8f88b8192c58d07a9dc1`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f840f93a8499fdb3efd112f5eedcef4290ba5edc497321ae223cdfc4dcb80e`  
		Last Modified: Fri, 27 Aug 2021 00:19:58 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:7b1ad12d6c6e44e24975eb80e1111d97db29e82416a00dadd5e14a67bf6c0ae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull nats@sha256:f6699a354c1c84d5ad72289d99c815e7bf11f983cd786684a5015745992e58e4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6276264126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af044355ba3348cfc4c9fb174c578e012f1a979a5d04b3681aafc9c2d9411eff`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 25 Aug 2021 13:59:32 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 25 Aug 2021 16:08:06 GMT
ENV NATS_DOCKERIZED=1
# Fri, 27 Aug 2021 00:16:54 GMT
ENV NATS_SERVER=2.4.0
# Fri, 27 Aug 2021 00:16:55 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.4.0/nats-server-v2.4.0-windows-amd64.zip
# Fri, 27 Aug 2021 00:16:56 GMT
ENV NATS_SERVER_SHASUM=6c66acf5ed7e87a1ed9c499033c8c64c8c1365c5a95973ec57859abf1a69b032
# Fri, 27 Aug 2021 00:17:57 GMT
RUN Set-PSDebug -Trace 2
# Fri, 27 Aug 2021 00:19:20 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 27 Aug 2021 00:19:21 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 27 Aug 2021 00:19:21 GMT
EXPOSE 4222 6222 8222
# Fri, 27 Aug 2021 00:19:22 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 27 Aug 2021 00:19:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a869803fc3d8292f0fe1bc6ed35e1ceedbd7c797a1486767a55f88c6c28ed4c5`  
		Last Modified: Wed, 25 Aug 2021 15:45:25 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a745f96c10790ef3a2006dbd4c116eb2f1552fd3c4a38fca179a8160e9918ac1`  
		Last Modified: Wed, 25 Aug 2021 16:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbc2c744fbea737586b320c08b480fbd8eb2dc994300a74c6a4864ee082901`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530ba921538bcf67912fb5a5d6794e991501dbca08ae8137712fc58854f4f68`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35523016d41ba152afbfa0a809770805058865f49d17d6d04d77fab412e5c29d`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348276d7a124485ea8bc7bad9b9147c84dd20fda1da976a1542cbdb907e4ea95`  
		Last Modified: Fri, 27 Aug 2021 00:20:37 GMT  
		Size: 336.1 KB (336071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751871e4a816cbaed81ad603047b0c9b536c2180dd5e54f7874d1ca37ef57851`  
		Last Modified: Fri, 27 Aug 2021 00:20:36 GMT  
		Size: 4.9 MB (4948899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9507c0638be8fdbc5f10f76a31d751acfd94e02618ac7528b4856051bb3721`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 2.0 KB (1979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784f2e48cdd62d72893e3cf7316c3c7764e937b9ccade0cb0ce5547ee1e1a304`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ba660ed14d0923ea760b909e13fa4ff5bc4fe34acc4e9b0e5e072b2cd9704`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34329777aaf85af2b82ec6fa6640f757cc9589247f7fe67e427a4e39c19bda`  
		Last Modified: Fri, 27 Aug 2021 00:20:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
